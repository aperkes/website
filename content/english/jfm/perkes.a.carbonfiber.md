---
title: "How not to make carbon fiber electrodes"
date: 2022-07-27T11:07:10+06:00
author: Ammon Perkes
image : "images/blog/blog-post-1.jpg"
bg_image: "images/featue-bg.jpg"
categories: ["Neuroscience","Electrophysiology"]
tags: ["Carbon Fiber","Electrodes","Electrophysiology","3D Printing"]
description: "I tried to make a new carbon fiber electrode"
draft: false
type: "post"
---


In pursuit of stable, long term neural recordings, I tried to implement and improve Tim Gardner's carbon fiber [electrodes](https://iopscience.iop.org/article/10.1088/1741-2560/10/4/046016/meta). In retrospect, I should have just worked harder to find a place to print the original. 


I had some initial difficulties getting mounting the electrode in a way that was accurate during implantation, but the larger problem was the 3d print supplier they had used would no longer print the piece for a price we could afford. 

I decided to try to make a cheaper, simpler version, easier to produce version. I got lots of 3d printing experience, but ultimately never got one that worked in a bird's brain. 

I first tried to just pass the electrodes through a simple grid [seen here](https://github.com/aperkes/Failedcarbonfiber/blob/main/CF%20electrode%20BOTTOM%20v8.STL), bundle them using water (per Gardner's approach), then put a cap on top. First I tried with a flat cap, but water didn't bead off properly and it always got stuck. The cap was also very difficult to get on, and I tended to break the electrodes. 

I then tried a single piece [(seen here)](https://github.com/aperkes/Failedcarbonfiber/blob/main/Bottom%20RHD%20v11.stl). This was pretty beautiful, but without the little point to hold it together, my memory is it wasn't sturdy enough, and also fire-sharpening the electrodes turned out to be extremely difficult. 

From there I tried to make a piece that would essentially work like the Gardner original, but would be easier to produce because it would come in two parts and then snap together. [picture here](https://github.com/aperkes/Failedcarbonfiber/blob/main/mark7_1_bottom.stl)

At this point I was also frustrated by how it was impossible to know which electrode was which (which was a problem for my planned experiments), so I switched to a straight shaft design. I was using these amber microfilaments, threading the carbon fiber elecrodes through them and glueing them into the 3d printed piece. 
This showed some promise, I was able to get it into brains a few times, although the manufacture process was very difficult and time consuming, and firesharpening was again challening because the individual fibers would sometimes meld together, because they were so close. 

Because the electrodes weren't bundled, I used PEG (per [Patel's method](https://iopscience.iop.org/article/10.1088/1741-2560/12/4/046009/meta?casa_token=aNG_v-GBlYsAAAAA:7GGCcHADXeRWEWdN1ospRHlSyr46T67wuts4GluLCBY_c3rck1yHntZnrMLMIjJUPOLGRpSRtg) to provide stiffness. 
This worked reasonably well actually, although I found it quite difficult to control the PEG dissolving process during implantation. 

I also had a lot of difficulty with mounting the pieces, as well as visualizing the brain as they were entering. 
I made some 3d printed files to hold the pieces, and that helped, although visualization was still a challenge. 
I ended up using a dentist mirror to make sure I could get a good look at all sides as it was entering the brain to avoid buckling. 

These latter methods showed some promise, however I had run out of time to develop electrodes, 
so I threw in the towel. 

## My take: 
Carbon fiber electrodes show a lot of promise for long term recordings, however looking at the literature, 
few if any labs have been able to publish actual results, rather than proofs of concept. 
If your particular question demands low impact, long duration recordings, it is definitely worth considering, 
however I would say that they are very much in their "beta testing" phase. 

If you can use some other, more established approach, I recommend it. 

[repo of stl files](https://github.com/aperkes/Failedcarbonfiber)

