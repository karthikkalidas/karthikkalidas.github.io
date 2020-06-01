---
title: "Modeling Autonomous Vehicle Interactions with Pedestrians"
permalink: "/portfolio/pedestrianAV"
layout: "single"
date: 2020-05-15
toc: true
toc_label: "Contents"
---

## Introduction
<img src="{{ "/images/projects/pedestrianAV/intro.jpg" | absolute_url }}" width="30%" hspace="20" align="right"> Autonomous vehicles (AVs) must share space with human pedestrians, both in on-road cases such as cars at pedestrian crossings and off-road cases such as delivery vehicles navigating through crowds on high-streets. Unlike static and kinematic obstacles, pedestrians are active agents with complex, interactive motions. Planning AV actions in the presence of pedestrians thus requires modelling of their probable future behaviour as well as detection and tracking which enable such modelling. This is especially even more safety critical in edge case scenarious such as driving through occluded areas, limited vision driving such as during night, and while encountering crosswalks at corners and intersections. Thus these situations make the challenge of motion prediction of other dynamic obstacles a hot topic, pedestrians an even more crucial one. There has been significant progress in research towards predictions for other vehicles in the scene but not quite extensively done for pedestrians specifically. This is mainly due to the complexities of pedestrians, with added uncertainty and quick unpredictable manuevers. In case you want to learn more, make sure to check out Oliver Cameron's blog [Let Me Level 5 With You](https://olivercameron.substack.com/p/the-next-leap-in-self-driving-prediction) on Predictions.

## Objective
![](/images/projects/dashev/adl.jpg)

At ADL, our goal is to deploy shuttles to service at different parts of the city of Columbus for soft autonomous driving, helping people in deliveries and other basic essential needs. This project mainly focuses on the operation of shuttles at the Ohio State School for the Blind. The main objective is to develop autonomous shuttles which are capable of operating safely in a blind school environment in the presence of impaired vision pedestrians, helping them commute across different parts on the school at there will. My goal specifically is to develop algorithms which can help detect, track and predict the motion of such a mixed crowd of people. These motion predictions will be used to develop path planning strategies which can enable robust safety during such interactions. The generated paths need to ensure collision-free trajectories and evasive manueverability if required.

## Methods

We start the project with a pedestrian model to be developed. This is one of the crucial steps which will help us predict the future motion of a pedestrian reliable using bayesian techniques. There are several constant velocity based models already developed in literature and taking inspiration from those would be a good starting point for future development.

![](/images/projects/pedestrianAV/pedestrian_model.png)

The steps would be to first detect multiple pedestrians in the near enviroment, recognize their future intention using Intent Prediction models. The next step is a challenging one and is a active area of researh - Multi-Target Tracking (MTT) to track all the different numerous pedestrians observerd. Once we all the pedestrains being tracked, we would try to predict their future trajectories. These future trajectories would be used to compute the expected Time-to-Collision (TTC). The methods can be optimized to consider only the pedestrians which pose greater risk to the vehicle and therefore some sort of a risk-based approach can be undertaken. The TTC to all the nearby pedestrians can be taken into account to plan the future trajectory of the vehicle which minimizes risk. This can be a simple emergency braking of an evasive manuever when just braking would not suffice. The loop continues by computing the next closest TTC which poses the greatest risk.

## Simulation and Testing
Coming Soon!

## References
- [1] Jens Kotte, Carsten Schmeichel, Adrian Zlocki, Hauke Gathmann & Lutz Eckstein (2017) Concept of an enhanced V2X pedestrian collision avoidance system with a cost function–based pedestrian model, Traffic Injury Prevention, 18:sup1, S37-S43, DOI: 10.1080/15389588.2017.1310380
- [2] F. Camara et al., “Pedestrian Models for Autonomous Driving Part I: low level models, from sensing to tracking,” Ieee Trans. Intell. Transp. Syst., vol. X, no. X.
- [3] E. Chao, “Autonomous Driving : Mapping and Behavior Planning for Crosswalks by,” 2019.
- [4] A. Rasouli and J. K. Tsotsos, “Autonomous vehicles that interact with pedestrians: A survey of theory and practice,” IEEE Trans. Intell. Transp. Syst., vol. 21, no. 3, pp. 900–918, 2020, doi: 10.1109/TITS.2019.2901817.
- [5] C. Scholler, V. Aravantinos, F. Lay, and A. Knoll, “What the constant velocity model can teach us about pedestrian motion prediction,” IEEE Robot. Autom. Lett., vol. 5, no. 2, pp. 1696–1703, 2020, doi: 10.1109/LRA.2020.2969925.
- [6] L. P. Robert, “The future of pedestrian-automated vehicle interactions,” XRDS Crossroads, ACM Mag. Students, vol. 25, no. 3, pp. 30–33, 2019, doi: 10.1145/3313115.
