---
layout: page
title: Semi-autonomous Mobile Robot
description:
img: assets/img/510_3D_CAD.png
importance: 6
category: work
---

Built an autonomous mobile robot that is controlled using a ESP32 and performs the following tasks:

1. Wall Following:
A proportional controller is used to maintain a certain distance from the wall while following it and the sensors used are ultrasonic sensors and time of flight sensors.

2. Remote Control: 
Remotely controlled using UDP protocol.

3. Following a flashing beacon:
IR sensors are used to detect a beacon (made of IR LEDs) and approach it.

4. VIVE localization:
A diode is used to capture the laser sweeps from HTC VIVE base stations and localize the bot in an arena.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/510_actual_bot.jpg" title="Poster" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    First iteration of the bot
</div>