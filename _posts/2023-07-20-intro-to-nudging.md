---
layout: post
title: Nudging as an Optimizing / Accuracy Increasing Process
subtitle: Explaining Earth System Models of Intermediate Complexity (EMICs) -- Part 7 (Nudging)
# cover-img: /assets/img/path.jpg
# thumbnail-img: /assets/img/earth.jpg
# share-img: /assets/img/path.jpg
tags: [modeling, climate]
---
# Nudging

Model instability for values within a studied range is exceptionally rare. However, deep learning algorithms do tend to develop bias during their training, so a common tactic of nudging is usually coupled with the implementation of a deep learning algorithm in climate models. Nudging arises from our knowledge of what a climate model should look like. Climate modelers and common sense holders alike understand that an RCM should not present significantly different results from the driving (GCM) model. Using nudging, we can keep the RCM model from differing too strongly from the surrounding model. Nudging is done by tweaking the initial values of the model and by normalizing the values output during each "tick" of a model run, keeping them between some range of values. For instance, it would be unreasonable to see a patch of land warm 20 degrees celsius in one year, a result like this would probably be counted as extraneous. Unsurprisingly, nudging a climate model towards intended outputs can increase accuracy, especially at finer resolutions.
Nudging takes on extra importance when deep learning is integrated into the models being run, for deep learning models struggle to make predictions on values outside of their training set. The study of deep learning model performance in out-of-dataset values constitutes its own body of literature, but even in EMIC research there is a growing body of deep learning focused research in this direction. A paper from the Allen Institute for AI was published in 2022 studying different methods of extremum detection in deep learning models being applied to climate modeling. Notably, nudging is not generally needed in larger models (GCMs) (i have a cite for this), which affirms that our understanding of the climate system is mostly correct.
