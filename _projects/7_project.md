---
layout: page
title: Ensemble Kalman Filter
description: 
img: 
importance: 7
category: robotics
---

In time critical systems, it is essential that the state estimation pipeline is quick and accurate. Current methods often struggle to achieve both. In this project we attempt to rectify this problem by constructing an ensemble filtering method by combining the state estimates from multiple filters to get a better overall estimate. The ensemble consists of fast, weak learners that can compete with an accurate, but slow filtering algorithm. There are 3 methods to form the ensemble: a simple average, a perceptron network, and a dense neural network with loss functions of MSE loss and a custom loss function. We demonstrate that the performance of the ensemble, in specific the dense neural network, is better than the individual performance of each filter tested on the EuRoC dataset.

<a href="https://github.com/pranavpshah/Projects/blob/main/Ensemble_Kalman_Filter/Final_Project_Report.pdf">Report</a>

<a href="https://github.com/pranavpshah/Projects/tree/main/Ensemble_Kalman_Filter">Github Repo</a>
