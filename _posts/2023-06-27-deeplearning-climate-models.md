---
layout: post
title: Deep Learning as an Optimizing Process in Climate Modeling
subtitle: Explaining Earth System Models of Intermediate Complexity (EMICs) -- Part 6 (Deep Learning / Optimization)
# cover-img: /assets/img/path.jpg
# thumbnail-img: /assets/img/earth.jpg
# share-img: /assets/img/path.jpg
tags: [modeling, climate]
---
# Introduction to Deep Learning & Optimization Techniques
	
A growing body of climate modeling research is attempting to infuse “deep learning” into the mechanisms of climate models. In theory deep learning could offer a computationally efficient way to represent certain processes more accurately. Especially for processes that are currently parameterized, deep learning algorithms present an opportunity to create computationally efficient code to represent complex systems. Deep learning could offer a way to improve all forms of EMICs. Beyond deep learning, many of these optimization techniques will result in small, but significant, inaccuracies. As the model runs these inaccuracies build up, so a technique known as “nudging” is used to keep the values within a reasonable range. In this section we will discuss current work and potential pitfalls with both key climate modeling components.

## Deep Learning
	
Deep learning is a process by which a computer trains a set of “weights” to transform an input into an output. Deep learning models are trained with a task in mind and the weights are altered so that any given input produces the desired output. One of the most famous examples of deep learning is GPT3, or its big brother GPT4, aka. ChatGPT. In GPT4’s case, the model is trained with more than a trillion parameters. Training these models requires humongous amounts of compute time and energy, but once the weights are trained, they are relatively less difficult to use. The compute required both to train and run these models decreases exponentially, however, with their size. In the context of climate modeling, deep learning models are much smaller, and generally require very little energy to make predictions with, although they still require much more operations to be done than a simple linear computation.  
One potential issue with deep learning that is often discussed is incomprehensibility. Deep learning models are often considered, colloquially, to be “black boxes.” Because their structure is defined by layers of matrix multiplications their weights in their algorithms don’t contain actual meaning. Deep learning algorithms do not keep track of units or understand, inherently, the laws of thermodynamics such as conservation of energy. These are things that they must be taught, either explicitly or implicitly. This means that while studies may find that deep learning in some situations has created a more efficient and accurate climate model, it is hard to study the limitations of that model. Even if a range of values is determined where the model works well, without testing every value in the range it is possible there exists a set of values where the deep learning algorithm fails horrendously.  
