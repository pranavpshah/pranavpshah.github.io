---
layout: page
title: Autonomous VIO-based Quadcoptor
description: Developed and implemented the autonomous stack for a quadrotor
img: assets/img/Crazyflie2.0-585px.jpg
importance: 2
category: work
# giscus_comments: true
---

The autonomous stack for the a quadcoptor was developed and implemented in simulation and on a real drone. The stack was implemented on a <a href="https://www.bitcraze.io/products/old-products/crazyflie-2-0/">Crazyflie 2.0</a> drone. The graphical representation of the stack is as follows:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/vio_drone_stack_graph.png" title="Autonomous Drone Stack" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Graphical representation of the autonomous drone stack.
</div>

The different elements of the stack are as follows:
1. Controller: 
The controller implemeneted is a geometric controller. The idea behind this control is to align the z-axis along the desired force vector. It has two nested PID controllers, a position controller and a attitude controller. The attitude controller is tuned to respond atleast an order of magnitude faster than the position controller. 

2. Path planning:
The 3D space was discretized into voxels and different graph based path planning algorithms were explored like Dijkstra's algorithm and the A* algorithm. The quickest and optimal solution was obtained from A* algorithm. 

3. Trajectory Generation:
In order to generate smooth trajectories for the quadrotor, a minimum snap trajectory was implemented inspired from this <a href="https://ieeexplore.ieee.org/document/5980409">paper</a>.

4. State estimation and Localization:
A VIO (visual intertial odometry) algorithm was implemented which uses stereo images for state estimation and localization of the drone. 

The stack was extensively tested in simulation on several different maps to ensure that the drone can navigate through different obstacles reliably.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/vio_sim_op1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/vio_sim_op2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/vio_sim_op3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Simulation result of the drone flight in 3 different maps.
</div>
