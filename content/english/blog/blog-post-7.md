---
title: "mobileSrc documentation is live!"
date: 2025-10-17T11:07:10+06:00
author: Ammon Perkes
image : "images/blog/blog-post-7.jpg"
bg_image: "images/featue-bg.jpg"
categories: ["News"]
tags: ["Code"]
description: "Why did the chef leave his job at the diner?"
draft: true
type: "post"
---

We always get asked how we a) track our videos and b) record our fish. In a future post I’ll outline our main tracking pipelines, but I’m excited to share that our recording pipeline is fully documented and available on github! This includes all of the raspberry pi code that keeps things running smoothly, as well as the code for a supervisor computer that checks for errors and processes videos each night. Some of this will certainly need to be adapted for your specific system (based on your storage situation), but this is a fairly robust toolbox for recording, and it comes with complementary fish jokes.

All schedules are maintained via a single file in the cloud, so there’s no coding ability required to update your schedule. By far my favorite feature is mosaic.sh, which grabs still from every video from the previous day and overlays them (in our case, in real-world configuration) so that you can quickly spot any problems in your recording before they disrupt your experiment. Probably more importantly, the pi’s and supervisor computer constantly check to make sure the videos are growing and send a message to slack if their video stops for any reason, afterwhich they reset themselves and turn the camera back on. We went from losing days of videos everytime there was anyproblem with a raspberryPi to (occasionally) losing minutes. Again, you will certainly need to modify this code to suit your specific layout, but check it out! It might save you some headaches.

