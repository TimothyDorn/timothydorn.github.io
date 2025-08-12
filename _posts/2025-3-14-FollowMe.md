---
layout: post
title: Follow Me Robots
excerpt: Methods of controller-less control of drones
published: false
---

We are entering a new world of robotics, but until they can fully control themselves, how can we direct them?

For hands-free control, follow-me robots are an exciting prospect. Let me explain how it works: a robot follows something (like a person). Pretty simple. This is an especially attractive solution if the followee has their hands occupied and can't use a controller.

Unfortunately, actual implementation is more complex. The reason is precision. To effectively follow a moving object you must know the relative distance between the follower and the followee, and the follower must know what it is following. 

Once again, this sounds simple, but if you have ever tried to follow someone through a crowd, or tried to estimate how far away something is from you just from eyesight you may understand some of the challenge.

One solution is if both objects have an "absolute" position, measured via some external point of reference, with data transfer between them. Another is really good sensors, that can track an oject reliably, and precisely measure distance. Or some combination of both good local sensing and relative positioning. The task is by no means impossible, but trade-offs do need to be made.

Let's take a look at some options:

### GPS ###
This is very doable, especially with the precision of modern GNSS technology. If you have one GNSS receiver on your follower and another on your followee you can simply adjust your robot's actuators to achieve the desired follow distance - implementation of actuation control is left to the reader. The real challenge is GNSS accuracy and precision. The accuracy isn't as important if the same relative inaccuracies apply to both receivers. It doesn't matter if the GNSS localization is off my a kilometer if both the follower and followee are off by the same kilometer. What matters much more is precision. If your robot is supposed to follow one meter behind you but has the precision of several meters it might be able to follow in your vicinity, but won't be able to maintain a steady distance.

Adding GNSS Real-Time Kinematic (RTK) positioning can improve things, with centimeter or even millimeter level precision and accuracy, at the cost of needing a fixed base station. But this brings us to the biggest disadvantage of satellite based positioning - it only really works outdoors with few overhead obstructions. RTK systems can correct for errors coming from sending signals through the atmosphere, but not through roofs and buildings. An indoor GPS repeater may be able to help, but what if you want your robot to follow you no matter where you go, even without GPS signal? 

### Computer Vision ###
Computer vision based systems are the go to for fancy robot startups at the moment, and they have plenty of potential. From a biomimetics standpoint, most large terrestrial animals have already implemented vision based following. With enough ambient light, sensors (like eyes and cameras) can estimate distances between the sensor and the target. Especially if multiple sensors are used, allowing for triangulation.

The big challenge is developing the software. Machine learning algorithms need to be trained on large amounts of images and video to effectively differentiate a human from their surroundings, so the training data should include a variety of locations for the technology to perform consistently. These algorithms also need to consistently follow the same target, not just any human walking by. Identifying someone no matter which direction they face, even in a crowd of people, can be challenging even for humans with millions of years of evolutionary training data. If the target is not a human, but user defined, that is even more training data. 

As long as there is ambient light, clear sight lines, distinguishing features between potential targets, and plenty of training data, computer vision will likely remain the go to for follow-me systems for the forseeable future. While this does solve the issue with GNSS not working indoors it does not solve every use case. There are still other options.

### Wireless Communication RTLS ###
Real time location systems (RTLS) operate by measuring the distance between a transmitter and receiver using radio frequencies. Several different frequencies and protocols are currently being pioneered for precision localization, including Bluetooth Low Energy (BLE), Wi-Fi, 
