---
title: Pi, Frenchmen, and Gravity
updated: 2017-3-21 11:58
excerpt: Pi Day post! The strange relationship between pi and gravity, and how the French caused it
---

### Pi Squared

Take out a calculator ([or open google](https://www.google.com/search?q=pi+squared&oq=pi+squared&aqs=chrome..69i57j69i59j69i61l2j69i60.2193j0j1&sourceid=chrome&ie=UTF-8)) and enter 

$$ {\pi}^2 $$

you should get something like

$$ 9.8696 $$

Now if you're a gigantic physics junkie this number should immediately strike you as familiar. As it turns out, $$ \pi^2 $$ is incredibly close the acceleration due to gravity at the surface of the Earth, $$ g $$, which takes on a value of about $$ 9.81 \frac{m}{s^2} $$. In fact, there is only about $$ .5 $$% error between the two values.

At first glance, this seems like it should be a complete coincidence. After all, how does the ratio of a circle's circumference to its diameter have anything to do with the acceleration of gravity on some unremarkable hunk of rock floating in a vast universe? Moreover, $$ g $$ isn't even constant. It varies as you change altitude, latitude (due to the centrifugal force of the Earth's spinning), and location (due to variations in densities of the Earth's crust). And to top it off, $$ g $$ has units of $$ \frac{m}{s^2} $$ while $$ \pi^2 $$ is unitless.

Then again, $$ \pi $$ does seem to pop up in some of the most unexpected places. For instance, $$ \pi $$ appears in [the probability that any two randomly choosen integers are coprime](https://www.youtube.com/watch?v=RZBhSi_PwHU&t=639s), [Euler's identity](https://en.wikipedia.org/wiki/Euler's_identity), and physical constants, such as the [permeability of vacuum](https://en.wikipedia.org/wiki/Permeability_(electromagnetism)).

There is in fact an explanation and oddly enough it actually has to do with Frenchmen.

### The French Revolution

The French Revolution began in 1789, bringing with it far-reaching social and political changes. These changes were based on the Enlightenment phiolosphy of reason and equality. Perhaps one of the most significant changes (and the key to our mystery) was the adoption of the metric system—a system of measurement that resonanted with the enlightenment thinkers of the time in that it was not tied to a specific person (such as feet, based on the length of a king's foot) but was accessible to anyone and everyone.

### Math and Physics!

The metre was defined to be the length of a pendulum such that a half swing was one second. Now this doesn't seem to have much to do with $$ \pi $$ or $$ g $$, but let's look at this equation that relates a pendulum's period to its length (for small angles).

$$ T = 2\pi \sqrt{\frac{L}{g}} $$

Now let's substitute our definitions in. That is we'll but in $$ 1m $$ for $$ L $$ and $$ 2s $$ for $$ T $$ (as two half-swings should be two seconds).

$$ 2 = 2 \pi \sqrt{\frac{1}{g}} $$

Now with a bit of rearrangement we get

$$ \pi^2 = g $$

So there you have it. The reason why $$ \pi^2 $$ is so close to $$ g $$ doesn't have anything to do with circles or the earth or even gravity itself. Rather, it has everything to do with how we go about defining units. In fact, we could have made $$ g $$ equal anything we want, as long as we take care in defining our units!
