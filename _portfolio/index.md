---
title: "Portfolio"
layout: "collection"
permalink: /portfolio/index.html
classes: wide
toc: false
toc_label: "Contents"

feature_row_research:
  - image_path: images/projects/pedestrianAV/teaser.jpeg
    title: "Pedestrian-AV Interactions"
    excerpt: "How can autonomous vehicles predict a pedestrain's trajectory for safe maneuvering"
    url: "/portfolio/pedestrianAV/"
    btn_label: "Read More"
    btn_class: "btn--primary"

  - image_path: images/projects/simulation/carla_teaser.jpg
    title: "Creating Simulation Environments using Carla"
    excerpt: "Simulation environments are crucial for the testing of algorithms"
    url: "/portfolio/simulation/"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_kpit:
  - image_path: images/kpit2.png
    title: "Internship at KPIT Technologies"
    excerpt: "My experience being a part of the ADAS group at KPIT"
    url: "/portfolio/kpit/"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_racing:
  - image_path: images/team.jpg
    title: "Fomula Student : IIT Bombay Racing"
    excerpt: "My experiences in being part of Formula Student"
    url: "/portfolio/pp/"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_hobby_projects1:
  - image_path: /gifs/coursera_selfdr.gif
    title: "Coursera Self-Driving Car Specialization"
    excerpt: "Projects of State Estimation, Perception and Motion Planning for
    self driving cars. Part of the 4-Course Specialization"
    url: "/portfolio/coursera_selfdr"
    btn_label: "Read More"
    btn_class: "btn--primary"

  - image_path: /gifs/slam.gif
    title: "Lego Robot SLAM"
    excerpt: "Simultaneous Localization and Mapping (SLAM) project with a 2D robot environment"
    url: "/portfolio/legoslam/"
    btn_label: "Read More"
    btn_class: "btn--primary"

  - image_path: /gifs/lanefinding_video.gif
    title: "Lane Finding using OpenCV"
    excerpt: "Lane line detection for image and video streams using OpenCV and Python. Part of the Udacity Self-Driving Car Nanodegree program"
    url: "/portfolio/lanefinding/"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_hobby_projects2:
  - image_path: gifs/pp3.gif
    title: "Graph-Based Path Planning"
    excerpt: "Collection of Dijktra, A* and state-space based search algorithms "
    url: "/portfolio/pp/"
    btn_label: "Read More"
    btn_class: "btn--primary"

  - image_path: /images/projects/rl.jpg
    title: "Reinforcement Learning for Autonomy"
    excerpt: "Self-Driving Cars learn how to traverse through a racetrack using RL"
    url: "/portfolio/rl/"
    btn_label: "Read More"
    btn_class: "btn--primary"

  - image_path: /images/projects/ciy.jpg
    title: "Code-It-Yourself!"
    excerpt: "A collection of C++ games and applications"
    url: "/portfolio/ciy/"
    btn_label: "Read More"
    btn_class: "btn--primary"
---
## Research | Automated Driving Lab
{% include feature_row id="feature_row_research"%}
## Professional Experience
{% include feature_row id="feature_row_kpit" type="left"%}
## Engineering Experience
{% include feature_row id="feature_row_racing" type="left"%}
## Projects
{% include feature_row id="feature_row_hobby_projects1" %}
{% include feature_row id="feature_row_hobby_projects2" %}
