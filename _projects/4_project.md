---
layout: page
title: Transformer based neural-network for Human Trajectory Predicition
description: Attention based Transformer Network to predict human trajectories in a scene
img: assets/img/transformer_architecture.png
importance: 4
category: robotics
---

In this project, we implement the classical attention-based Transformer Network (TF) to predict the future trajectories of individuals in a scene. The project is inspired by the paper <a href="https://ieeexplore.ieee.org/abstract/document/9412190">"Transformer Networks for Trajectory Forecasting"</a>. We use the TrajNet dataset which is a superset of diverse datasets. Training on this dataset ensures that our model generalizes and performs well in unseen situations. We build our model using different optimizer and scheduler techniques and analyze the one that gives us the best performance. We then perform extensive testing using the best model and present some quantitative and qualitative results. The results show that our best TF model is able to predict future pedestrian trajectories with an average error of ~ 45 cm.

<a href="https://github.com/pranavpshah/Projects/blob/main/Transformer_model/ESE_546_Project_Report.pdf">Report</a>

<a href="https://github.com/pranavpshah/Projects/tree/main/Transformer_model">Github Repo</a>