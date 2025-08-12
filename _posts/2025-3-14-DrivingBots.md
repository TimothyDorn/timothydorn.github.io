---
layout: post
title: Driving Bots
excerpt: Remote control and autonomous UGVs
published: false
---
# {{ post.title }}

who - robotics designers
what - wheeled robot steering
where - manufacturing
when - steering regimes
why - control, utility
how - mechanical engineering, lateral thinking

sources: 
https://medium.com/@thiagohbaum/the-history-of-steering-mechanisms-part-2-18091c990f52

vehicles to exhibit:
dual wheel
tricycle
skid steer - weight distribution needs to be front loaded or rear loaded to minimize torque on wheels
6-wheel, 8-wheel differential steer (hanwha, mission master sp)
differential steer
omni-wheel fork lift, mecanum wheel
car (front steer) Ackermann 
military 8 wheel vehicle
forklift (rear wheel)
telehandler (front, all wheel, crab, semi-crab) https://www.zf.com/products/en/construction/products_64458.html
capra diamond wheel
articulated dump truck
articulated bus (pusher and puller) with front or front and rear steering
motor grader (steer and articulation)
Swerve Drive

In the hundreds of thousands of years than the human species has been around, wheeled vehicles are a very new invention. They were first developed closer to today than to the beginning of agriculture, and being such a recent technology, there is still much to explore in their design and development - in particular, the fascinating world of steering mechanism.

Particularly today, there are revolutions in vehicle design happening, with military and construction vehicles, ground drones, and electric vehicles all spurring and enabling advancement. But, for steering mechanisms in particular, knowledge of these advancements is unevenly spread across disciplines. This knowledge gap is most apparent and frustrating in the near uniformity of design of ground drones. Here are some examples:

To be clear on terminology, this article will use the term UGV to describe all uncrewed wheeled vehicles. Various terms the reader may be familiar with include Unmanned Ground Vehicle (UGV), Uncrewed Ground Vehicle (UGV), Unmanned Guided Vehicle (UGV), Automatic, Automated, or Autonomous Ground Vehicle (A-UGV), Automatic Guided Vehicle (AGV), Automated Guided Vehicle (AGV), Autonomous Mobile Robot (AMR). https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=927167 



In one of my previous roles (that I am unfortunately restricted from discussing in detail), I designed and built a variety of remote controlled construction vehicles, mainly for material distribution. Some of these vehicles were modifications of existing platforms, but some were built fully in-house.

These custom designs were fully electric, enabling drive systems that would be more challenging in a traditional ICE vehicle. A vehicle with four independent drive motors can do zero-point turns, use software defined wheel differentials, and four wheel drive with minimal mechanical complexity. The simple mechanics makes initial vehicle design easier - there are numerous robotics platforms available today many having similar designs - but that simplicity can itself limit the functionality. There is a gulf of opportunity that exists between the extremely complex - e.g. robot dogs and humanoids - and the extremely simple fixed wheel UGVs. Vehicles that fill the gap exist in other fields, but very few of them have been adapted to robotics. I will be exploring some of these designs below.

### Lateral Thinking with Withered Technology


