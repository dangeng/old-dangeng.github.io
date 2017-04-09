---
title: Three ways of looking at a riddle
updated: 2016-07-21 10:38
excerpt: Not going to lie, I spent a long time trying to come up with thirteen ways to look at this
published: false
---
### The Riddle

I first heard this riddle from a truly remarkable guy on a bus trip in the middle of the night and it goes something like this:

_There are N light switches in a room that each connect to N lightbulbs in another room. You happen to want to know which lightbulb is connected to which light switch. You can do this by turning on or off whichever light switches you want, and then entering the second room to see which lightbulbs have been turned on. So given N lightbulb and ligh switch pairs, what is the least number of times you must enter the room to figure out exactly which switch connects to which lightbulb? (This is not a trick question: you cannot see in to both rooms at once, you cannot feel the lightbulbs to detect warmth, and you can't follow any wires.)_

I've posted the three ways that I've found to look at this riddle well below this paragraph (to avoid any spoilers!). Just scroll down when you're ready to see them. Also, if anybody has any other way to approach this riddle, I would love to hear it. I really want to try to get to thirteen!

+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 
+ 

### 1. Information Theory

The first way to approach this riddle (and possibly the cleanest) is to use information theory. Think of it this way: if we number the light switches and we can then assign each lightbulb a number corresponding to its switch. Then we simply want to find out what number each lightbulb is. Given N lightbulbs, each lightbulb would need FLOOR LOG N BASE 2 bits to encode its number. Well, each time we go into the room we should learn something new about a lightbulb. Thus, each time we go into the room, best case scenario we should get 1 bit of information for each lightbulb. Because the largest number is N, we need a maximum of FLOOR LOG N BASE 2 trips into the room to figure out which bulb is connected to which switch.

### 2. Recursion

Well, we have an answer to the riddle. But it should feel slightly uncomfortable that we just _assume_ each time we go into the room it's possible to get a bit (in the information theory sense) of information for each bulb. What we need is a heuristic for choosing which switches to switch. To do this, we'll use a bit of recursion.

Let's say, for the sake of argument, that we have $$ 2^n $$ bulbs, where $$ n $$ is an integer. The first step to take would be to turn on exactly half of the switches. Something like this:

<center>
	<img src="/assets/riddle/switches-1.png">
</center>

Where the red circles are on switches and the black circles are off switches. What information have we gained from this? Well, we now know that each switch must belong to a group of four, instead of eight now. The bulbs that turn on must belong to the group of on (red) switches, and the bulbs that stay off must belong to the group of off (black) switches. Essentially, we have gained a single bit of information for each bulb by reducing the possibilities from 8 to 4.

The next step would be to do the exact same thing (recursion!). We take one of the groups of four and only turn on two of the switches. Something like this:

<center>
	<img src="/assets/riddle/switches-3.png">
</center>

Thus, by going into the room and looking at which bulbs turn on, we can take the group of four bulbs and four switches and reduce them down to two groups of two. We've gained one bit of information for the first group of four! We could then take the other group of four, turn on two of the four switches and get two more groups of two. However, notice that this step can actually be done concurrently with the other group of four. It would look something like this:

<center>
	<img src="/assets/riddle/switches-4.png">
</center>

Finally, by recursing one more step and turning on the following switches:

<center>
	<img src="/assets/riddle/switches-5.png">
</center>

Thus for 8 bulbs, we need FLOOR LOG 8 BASE 2 = 3 trips in to the room. And in general we need...

### 3. Discrete Fourier Transform

The final (and in my opinion the most illuminating) way to look at this is to realize each time we go into the room we switch on switches in a pattern of a discrete fourier basis. This basis "spans" the set of 
