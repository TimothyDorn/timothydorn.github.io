---
layout: post
title: Wearable Latching Actuator
excerpt: Methods of controller-less control of drones
---

My master's thesis concerned the design, development, and evaluation of latching mechanisms. Specifically, latches designed to be used with artificial muscles in wearable applications.

### Purpose
Research has increasingly begun to focus on a class of biomimetic linear actuators known as artificial muscles. While this research has shown promise, contemporary artificial muscles have a variety of drawbacks, such as the need for high voltage, high current, or high fluidic pressures, depending on the class of artificial muscle. These drawbacks result in large power requirements, and consequently either large battery packs or short term usage, reducing the wearability or mechanical utility of the artificial muscles.

One method to reduce power requirements is to use an actuated latch. Such latching devices do not change the intrinsic properties of contemporary artificial muscles, but serves as a complimentary technology to increase the utility of artificial muscles in wearable systems. Specifically, latching devices enable the short term use of artificial muscles in applying a desired actuation force and displacement, then allows said artificial muscle to be powered off without loss of applied force or displacement. Such a system decreases the long term energy requirements of wearable actuators, provided high frequency actuation is not required.

### Design and Construction
Three different latching designs were built and tested, based off of a gear and pulley system; a ratchet design; and a toothed cam. 

Each latch was designed with wearability in mind. Guidelines for wearability were used as reference. The primary design choice in facilitating wearability was to keep the latches as small as possible given resource and manufacturability constraints. In particular, the height of each latch, measured normal to attachment point, was minimized in an attempt to keep each latch within the wearers intimate proxemic space and perceived as an extension of their clothing/body. Small and rigid latch designs were favored over compliant designs due to the perceived challenge of designing a compliant latch system capable of precise and repeatable latching.

To facilitate ease of attaching each latch to a garment, all three latches were designed with the same mounting points consisting of two textile friendly metal snaps. This type of fastener has been common in wearable technology research and provides a strong mounting point while being easily removable and unobtrusive. The small size and ease of integration of snap fasteners allowed the latches to be easily attached to nearly anywhere on the human body.

### Results
The belt and pulley design was found to have the most accurate force and displacement values, and was able to reliably latch and disengage for cable tensions up to 60 Newtons, surpassing the other designs. However, the design was the least wearable, being large and heavy, as well as more power intensive than the other designs.

The ratchet design was more wearable, and performed similarly to the motor design at low forces below 5 Newtons of cable tension. However, the ratchet design was less capable of holding force over time and the ratchet cable easily deformed, and was only moderately wearable. Despite these failings, the ratchet design was easy to manufacture with an extrusion 3D printer, making the design a good option for a simple wearable application requiring only small tensile forces.

The cam latch design was found to be similarly wearable to the ratchet design, but the rope used as the latch cable was compliant and flexible, making it the most wearable cable of the three designs. The cam design was also similar to the motor design for most metrics at small forces, however it suffered from high displacement due to the way the cam mechanism engaged with the cable and the high strain of the cam cable under small forces. The cam design required more precision manufacturing to function, and wear on the cam teeth quickly decreased the forces that the cam was able to hold. These drawbacks mean that the cam design was found to be most viable for applications prioritizing wearability above all else, and where higher manufacturing costs are acceptable.

The research demonstrates the viability of using latching devices in artificial muscle driven wearable robotic systems. Existing artificial muscles research has often focused on material science breakthroughs and novel innovations, while ignoring the well-worn technologies that have proved effective in wearable applications for centuries or millennia. This paper makes the case that next generation artificial muscles (high strength, low power, long lifespan, high frequency) are not needed for many contemporary soft, wearable robotic applications. Rather, latching systems make many low frequency wearable systems viable in the present day using existing artificial muscle technology

### Full Paper
You can access the full PDF of my thesis [here](/assets/Thesis.pdf){:target="_blank"}!