---
title: "Creating Realisitic Simulation Environments"
permalink: "/portfolio/simulation"
layout: "single"
date: 2020-03-11
toc: true
toc_label: "Contents"
---
## Introduction
Simulation has become a key technology for virtually testing a vehicle in a highly realistic environment that can mimic all weather conditions, lighting and city roads, down to the actual cracks in the road. The purpose of virtual testing is for the vehicle to “practice” driving in an environment almost identical to real-world conditions.

Simulation provides an opportunity for automakers to analyze what needs to be fixed or adjusted in the vehicle in a virtual environment, which creates a significantly safer vehicle before testing it on the road. In fact, each component of the vehicle, including the sensors that make up the driving system, is tested in simulation before it is implemented so that each component is optimal prior to installation. All this is done to ensure maximum safety precautions. The role of simulation in self-driving vehicles shaves off years of testing that would be required on the road since those same miles are driven in a fraction of the time in a virtual simulation.

I believe simulation is a key component to bringing autonomous vehicles to market. Shaving these years off of road testing and guaranteeing safety to a population that has never used or seen autonomous vehicles before is critical.


### CARLA Simulator
![](/images/projects/simulation/carla_teaser.jpg)

[CARLA](https://carla.readthedocs.io/en/latest/) (Car Learning to Act) is an open-source autonomous driving simulator. CARLA is grounded on Unreal Engine to run the simulation and uses the OpenDRIVE standard to define roads and urban settings. Control over the simulation is granted through an API handled in Python/C++ that is constantly growing as the project does.

### RoadRunner
![](/images/projects/simulation/roadrunner.jpg)

[RoadRunner](https://www.mathworks.com/products/roadrunner.html) is an interactive editor that lets you design 3D scenes for simulating and testing automated driving systems. You can customize roadway scenes by creating region-specific road signs and markings. You can insert signs, signals, guardrails, and road damage, as well as foliage, buildings, and other 3D models. RoadRunner provides tools for setting and configuring traffic signal timing, phases, and vehicle paths at intersections.


## Objective

![](/images/projects/simulation/teaser.png)

This work focuses on creating realistic simulation enviroments for autonomous vehicle seamlessly using Google Maps 3D and GIS data. The intuition behind this is to import google maps 3D data into a modeling software and use as a reference asset for building high definition road elements using RoadRunner. A realistic simulation enviroment offers several benefits in testing out perception algorithms and saves outdoor testing time to a great extent.

## Methods

For this purpose, I have used to Google3D [MapModelsImporter](https://github.com/eliemichel/MapsModelsImporter) tool by Elie Michel. Kudos to him for creating this easy to nifty tool.

We can now import the 3D mesh data into a popular modeling software such as Blender. Using the extensive features (Edit Mesh) that Blender has to offer, we can edit the models by removing crooked roads, coarse textures and all other assets that we don't want to be in our enviroment. I used this tool to remove the trees, roads and all the buildings which were modeled very crudely by google 3D. These assets can be replaced in RoadRunner for a more realistic enviroment. This is what I get at the end.

![](/images/projects/simulation/buildings.PNG)

Now we can move to RoadRunner for modeling the road elements. The model is imported into RoadRunner as an asset on top of the GIS data. The GIS data (available online on sites like USGS, etc.) is pretty useful for georeferencing the assets, and modeling roads relative to their geographic elevation. The Point-Cloud data can also be loaded for accurately placing the trees and other assets in the scene. Once the road modeling is done, we are ready to export the map into Carla. The only cumbersome step would be the post-processing of models in Blender which is difficult to automate. Voilà! We can now follow this procedure for creating whatever parts of the world we want to test our cars in.


## Results
The Ohio State School for the Blind is our ODD and was modeled using the above procedure. I am now working on improving the road elements and trees on roadrunner with reference to the GIS and Point-Cloud data. This realistic environment will be used in my pedestrian modeling research.

![](/images/projects/simulation/roadrunner_final.png)
