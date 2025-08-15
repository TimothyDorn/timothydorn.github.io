---
layout: post
title: Standing Desk
excerpt: Custom Standing Desk.
image: /images/pic04.jpg
published: false
---
# Building a Standing Desk
## A project for the brave and foolish.

"The youth gets together his materials to build a bridge to the moon, or perchance a palace or temple on the earth, and at length the middle-aged mans concludes to build a wood-shed with them." - Henry David Thoreau

It is with this unbound confidence that I set out to build a standing desk; bigger, stronger, cheaper, and more lovely than anything I could purchase outright. Now, looking back on the project, I proclaim confidently that on only one of those goals did I definitively fail. Seeing as the other three goals are either subjective or relative, and with no other standing desks in my house against which to compare, any final scoring of this project would be superfluos. I did, however, succeed in making a standing desk. So on that point I would rate my efforts at 100%, and nothing more need be said about it.

Now, if you are primarily interested in my desk, its engineering, and my nascent manufacturing prowess, I advise skipping to the main body of the text below where I go into the entire process in detail. But for those in less of a rush, and holding greater curiosity, there is another quote from Mr. Thoreau I would like to share with you. It comes from one of his personal, private journals which, as you may know, were scooped up and sold for profit after his death, and now people like myself quote from them. On July 14, 1852, in the same entry as the quote above, but separated by writings on yellow butterflies and slaty sky-blue blueberries, Mr. Thoreau wrote: 

"A writer who does not speak out of full experience uses torpid words, wooden or lifeless words, such words as "humanitary," which have a paralysis in their tails." 

I will do my best to avoid using the word humanitary in this article, and, seeing as I now have far more experience in the making of a stand up desk than I ever intended to gain, I will hopefully avoid any torpidity and lifelessness as well. I whould warn the reader though, I did not set out to gain any bountiful experience with this project. In fact I thought it would be rather easy, and if I had written an article back before I started I imagine it would have been a "wooden or lifeless" description of attaching some linear actuators to a desktop. But this is not that article. 

Perhaps you have come here thinking you will make a standing desk yourself, underestimating the task, as I did. Perhaps you came looking for an easy guide, but are now starting to have misgivings. If so, good. You have left the world of LEGO and Ikea behind. The only path forward is the one you are prepared to make yourself. Now, despite my warnings, this project was still enjoyable to work on. And though I do not recommend it to anyone who values their time or money, for a reader who wants a project that combines mechanical and electrical design, sensor integration, programming, and diy manufacturing, building a standing desk may be just the project for you. Whatever your goals, I wish you the best of luck!

# Designing A Standing Desk
I wanted to take the desk I already had and make it stand. Specifically, make the desktop stand, I didn't need the rest of the desk. I also wanted to make it sit, for those times where I value working and sitting. Looking on Amazon, there were a handful of standing desk legs for a few hundred dollars. With these I could take my desktop, screw it to the legs, and have a fully functional standing desk. But then I found some linear actuators for only $30. Why not simply attach the linear actuators to the desktop and save a couple hundred dollars?

These actuators were 12V, 5A, 20" stroke length, with a force of 1000N/220lbs, much stronger than any off the shelf standing desk legs. If the reader has any experience with linear actuators, they will hopefully already be saying to themself "that won't work" or "you haven't considered all the costs". To which I say "stop spoiling the story". One actuator at each corner would be more than capable of lifting and holding the roughly 15lb desktop and, as an estimate, the 200lbs of computer, display, paperclip, and human all sitting on the desk or leaning against the desk as they work. Commercial standing desks are generally rated to around 200lbs, the same as just one of my four actuators. I saw no flaws.

I 3D printed brackets to hold the linear actuators, screwed them into a wooden frame, then installed the linear actuators. A 12V 30A power supply ($45) was used to power the actuators. My hope at this point was for the desk to be fully analog, with one switch to power all four actuators at once, and four additional switches to power each leg. In theory, this would make the desk simpler, requiring a little extra wiring design in exchange for fewer parts and no coding. However, the actuators all extended at noticeably different speeds, and the electrical wiring needed to make the system analog required some specialty switches. Digital logic easily solves these problems, so the analog design was abandoned, but I continued prototyping using one analog switch per leg to verify the viability of the mechanical design.

We now return to the issue of using only linear actuators for the legs, an issue I should have recognized immediately. A linear actuator rated for a holding force of 1000N can support that force loaded along the axis of the shaft. However, they are generally several orders of magnitude weaker along the other two axes and require lateral supports to prevent bending and buckling. What this means for the desk is the actuators are more than capable of lifting the desk, but any horizontal or rotational loads risk snapping the legs and un-standing the desk. This is solved in commercial standing desks with telescoping tubes with tolerances tight enough to carry the lateral loads. Was this an option for my desk as well? Yes! I found some telescoping aluminium cylinders that could fit perfectly over my linear actuators, and with tight enough tolerances to provide lateral support. Did this completely negate the cost advantage of the linear actuators? Also yes. Whatever cost savings I had imagined at the beginning of this project were wiped out with this single purchase. 

To attach these tubes I 3D printed brackets to secure the outer tube to the desk frame. I also printed a spacer to go at the top of the leg between the tube and the linear actuator nested inside. These parts secured the outer leg in place horizontally. The inner tube was allowed to slide freely. Bottom stops were placed in each of the inner tubes for the actuators to press against, preventing any lateral movement of the tubes along the ground from imparting a moment on the actuators. With a four inch overlap between the inner and outer tubes at max stroke length, the problem of buckling was solved. Compared to a commercial standing desk, my build was a little more wobbly (at least compared to the solid steel frame designs available from high quality companies) and uses noticeably louder motors. Part of the wobble was from the tolerance between the tubes, and part from how the actuators and tubes were attached to the desk frame, but neither was a big enough issue for me to rethink the design. The desk is strong, simply lacking in precision. Perhaps an opportunity for future improvement! The noise, however, was mostly out of my control. I leave it for the reader to consider if they are planning a similar project. 

# Refining A Standing Desk
With the structure of the desk finally safe it was time to work on the functionality. At this point the desk was operated with four switches, one for each leg. This was not ideal, especially when the legs all extended at different rates. 



 

"The best way is always the simplest. The attics of the world are cluttered up with complicated failures."
https://www.thehenryford.org/collections-and-research/digital-resources/popular-topics/henry-ford-quotes