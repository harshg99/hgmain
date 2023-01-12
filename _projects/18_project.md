---
layout: page
title: Assembly with Robot Arm
description: Assembling two objects under limited vision information via feedback from force torque sensors
importance: 2
img: assets/img/lbr_iiwa_arm/1.png
category: Fun
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/lbr_iiwa_arm/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Completed this projected as part of my undergraduate research opportunities programme(UROP) at NUS.

Industrial robots are widely used in assembly tasks in various industries. In order to perform these tasks accurately,
it is important to have a system in place that can recognize the objects that need to be assembled. One way to do this
is through the use of computer vision techniques, such as using a Kinect V2 sensor to identify the location of objects.
The Kinect V2 is a depth sensor that uses infrared lasers and a structured light system to create a 3D map of the environment.
By analyzing this map, it is possible to determine the location and orientation of objects within the environment.

In addition to object recognition, it is also important to be able to correct for any misalignments between the objects
that need to be assembled. This can be done using force torque sensing, which involves using sensors to measure the
forces and torques acting on an object. By analyzing these forces and torques, it is possible to determine the position
and orientation of the object knowing the objects geometry, and make any necessary corrections to align it with the target object.

Computer vision and force torque sensing can help industrial robots to perform assembly tasks more accurately and efficiently,
resulting in improved productivity and quality in manufacturing environments.

Check out the video at 

<iframe src="https://www.youtube.com/watch?v=efLT0cvJ2QY"
        width = "640"
        height = "480"
        frameborder="1"
        allowfullscreen>
</iframe


