---
title: A Light Puzzle
updated: 2016-11-21 11:43
excerpt: Here's a light puzzle that I've been thinking about
---

### Dimensionality

Let's consider the dimensions it takes to describe light. In computers, we can describe basically any color using the RGB color scheme. Each color is described using a tuple containing its red, green, and blue color on a scale from 1-255. For instance, Craylola's Razzmatazz has an RGB value of (227, 11, 92). Hence, Razzmataz is mostly red (227/255), and a bit of green and blue. This scheme allows us to represent just about any color, from jet black to bicycle yellow to wisteria to moonlight white. We can visualize it through this pretty neat cube, where the axes represent R, G, and B values.

<center>
	<img src="/assets/light/rgb.png">
</center>

So evidently, it takes three coordinates to describe a color. One for red, green, and blue. However, what about another way of representing light? What about representing light as a wavelength? Red light is about 700 nm and blue light is about 400 nm. In between 400 and 700 nm are the greens and the oranges and the yellows of the spectrum. Here's a visual of the spectrum method of representation:

<center>
	<img src="/assets/light/spectrum.jpg">
</center>

Using this method we have one dimension, but we're still missing the blacks and the whites and the greys. To get these colors, we can just add one more dimension: the amplitude of a light wave. Low amplitudes will correspond to darkness, or the absence of light, which we preceive as black.

So seemingly, with two dimensions we can completely describe a color that needed three dimensions to be described using RGB coordinates. So something's wrong. Either RGB is a redundant system, or the physically inspired system of wavelengths is missing a dimension. So which one is it?
