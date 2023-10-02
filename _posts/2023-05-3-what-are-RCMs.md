---
layout: post
title: What is an RCM?
subtitle: Explaining Earth System Models of Intermediate Complexity (EMICs) -- Part 2 (RCMs & Later Boundary Conditions)
# cover-img: /assets/img/path.jpg
# thumbnail-img: /assets/img/earth.jpg
# share-img: /assets/img/path.jpg
tags: [modeling, climate]
---

# Regional Climate Models (RCMs)

Regional climate models are a type of EMIC that focuses most of the computation on a specific region of the world. These models typically have an inner area where spatial (and sometimes temporal) resolution are finer and an outer area where the climate is simulated in very rough terms. Even for organizations that can afford to run a global circulation model, RCMs are vital. They allow researchers to run simulations in much higher density than can be done in a GCM. The Intergovernmental Panel on Climate Change (IPCC) uses RCMs to simulate paleoclimate data or generate higher quality predictions for areas where topography changes rapidly (e.g. the Alps). Although regional climate models are a form of EMIC and are generally less computationally demanding than a GCM, they are not always, and are sometimes just as demanding as a GCM. In these cases, they are run in a time-slice manner where predictions are made for short periods (e.g. 10 years) during any point in the future. These kinds of models blur the lines between GCMs and EMICs

## Lateral Boundary Conditions (LBCs)
	
The climate is an interconnected web of systems, if the entirety of the Amazon is deforested there will certainly be far reaching effects across the entire world, for example. As such, RCMs must simulate the entire globe's climate even if the intention of the researchers is not to examine a global impact. The area between the high resolution portion of an RCM and the lower resolution portion is named the lateral boundary. Many climate models take different approaches to specifying the “Lateral Boundary Conditions” (LBCs), often dependent on what the researcher is attempting to model. At a high level, the information passed over the boundary includes moisture, temperature, and wind direction. 
Of course, in areas where the boundary cuts across the ocean relevant data regarding the temperature and direction of the ocean currents will be passed as well. In practice, implementing this transfer represents a much more tricky and difficult endeavor. The IPCC’s 2007 (Working Group I) assessment of RCMs predicts that the salient problem for improving their accuracy in the future will be optimizing the performance of the LBCs. Many models employ a tactic called nudging to reduce accumulated error from the parametrizations used in creating the LBCs. For example, Collier and Mölg (2020) used nudging to create a high resolution dataset of climate conditions in Bavaria.