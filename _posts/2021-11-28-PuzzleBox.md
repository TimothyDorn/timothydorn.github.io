---
layout: post
title: Electronic Puzzle Box
excerpt: Puzzle box game.
published: false
---
For the Mechatronics class capstone project our team built an electronic puzzle box!

# Device Description:
Our device will be an interactive puzzle box for a player to solve. On the top of the box will be a
series of LEDs laid out in a cross shaped pattern. The puzzle box will challenge the player to
balance the box about a certain axis while simultaneously turning some knobs and pressing
some buttons in a proper order. Each playthrough of the box will be different, allowing players to
play multiple times without repeating what they did in previous games. The purpose of this
project is to update the age old concept of a puzzle box using contemporary technology.

# Technology
The puzzle box will contain a triple axis gyroscope that measures rotation of the box. The box
will randomly orient the z axis on each playthrough. The player will then have to tilt the box so
the x and y axes, as measured by the gyroscope, will lie orthogonally to the z axis. The player
will be able to see how they should tilt the box based on the LED display on the top. The LEDs
will be placed in a cross shaped pattern. When the box is tilted far away from the z axis the
lights at the edges of the cross will light up, but as the box is tilted closer and closer to the
correct orientation the lights closer to the center of the cross will light up, until the light in the
center of the cross lights up indicating that the box is positioned correctly. In addition to tilting
the box, the player will also have to turn on a secondary set of lights by positioning
potentiometers and pressing the right buttons. This will be randomly generated so each
playthrough requires different actions. All of these actions will be controlled by a PIC
microcontroller.

# Components
Part Name Model Number Manufacturer Source Cost ($)
Microcontroller PIC16F18446-I/P MICROCHIP Newark 2.20
Gyroscope L3GD20H Adafruit Adafruit 12.50
Potentiometers Any Any Any In kit
LED Any Any Any In kit

# Technical Risks:
The programming of the gyroscope is projected to be the most challenging part of this
assignment. Time must be spent on finding libraries and gyroscopes that are compatible with
the PIC microcontroller, and additional time must be spent learning the libraries, testing, and
troubleshooting using the gyroscopes. Depending on the serial connection the gyroscope uses
we may also need to learn how to configure the microcontroller to use a serial connection that
we never learned in class.
