---
title: Tricking Neural Networks
updated: 2016-07-21 10:38
excerpt: Reading handwritten digits, predicting the stock market, driving cars, and diagnosing cancers are just a few things that artificial neural networks have been taught to do. This fledging field in artificial intelligence holds much promise and is prehaps one of the most actively researched branches in computer science
---
### Neural Networks

Reading handwritten digits, predicting the stock market, driving cars, and diagnosing cancers are just a few things that artificial neural networks have been taught to do. This fledging field in artificial intelligence holds much promise and is prehaps one of the most actively researched branches in computer science.

First, a primer of neural networks. Essentially, artificial neural networks are mathematical models based loosely on how actual biological brains work (for more technical details, Michael Nielsen's book [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/) is a good place to start). For now, we can think of them as being a sort of black box. We put some stuff in, math happens, and then some stuff comes out. Say we're trying to classify handwritten digits, such as these:

<center>
	<img src="/assets/tricking-nns/mnist-digits.png">
</center>

Well, the stuff that goes in would be the brightness of each pixel in an image, and the thing that comes out would be actual number in the image. However, this doesn't just happen automatically! You see, on the side of the black box/neural network is a ton of dials on it.