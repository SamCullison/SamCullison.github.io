---
title:   "Sliders Project"
layout:  project
image:   "/assets/img/Sliders Screenshot.jpg"
excerpt: "Fusion Designed Aluminum Sliders."
header:
  teaser: "/assets/img/Sliders Screenshot.jpg"
---

# Origin of the Sliders Project

The sliders project began after I rewatched Iron Man and saw Tony Stark's Arc Reactor. I thought the design would look great as an aluminum object and I set 
about creating the CAD and CAM to manufacture it with the CNC. However, this proved to be easier than I imagined and I decided to change gears and instead create two pieces which would fit together and spin against one another. As you see in the CAD below, in a location where one slider has a positive feature, the other has the corresponding negative. The tolerances were also adjusted to ensure that the pieces could slide with limited friction from the walls.

# CAD of the Sliders

<iframe src="https://vanderbilt1024.autodesk360.com/shares/public/SH512d4QTec90decfa6ec16ac4eb3967ad91?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Difficulties in Machining

The cylinder base of the slider also proved to be difficult to machine with out current equipment. The arc did not provide a sufficient base for the mighty jaws, which I learned the hard way. In the future this design will be changed to have a sort of X that spans both cylindrical bases, as to provide a solid, straight surface for clamping. 

Although the end product from the intial run is not what I wanted, I am happy with the finish being much better than those of my "custom cubes". Instead of facing off only with the 4 flute 3/8" square end mill, a proceding toolpath was generated to "clean it up". This path used a 7 flute 3/8" square end mill at a lower feed rate and will be used in future projects. 

One Slider after First Iteration:

<img src="/assets/img/Sliders Phto.jpg" alt="Slider Photo" style="width:500px;"/>

# Lessons Learned

* The importance of generating smart toolpaths for clean productions was emphasized to me through this project’s CAM. By leaving stock on the initial face and contour, I was able to generate finishing passes with different bits which guaranteed a much cleaner finish.
* Circles are harder than squares. In the past cube project, I was able to make one pocket selection and let Fusion do the rest. However, I found it difficult to generate an appropriate and efficient toolpath for the face features. In the end I used the chain selection for two different pocket paths (the initial used the 4 flute 1/8", and the second used a 1/16" ball end to mill out the narrow channels). 
* How to use the "simulate toolpaths" option effectively. Although my paths were creating the object I wanted, I obviously checked the simulate tab to ensure there were no points of potential bit breakage or time wastage. By doing this I was able to spot and correct a deep cut which would have broken the small 1/16" bit immediately.
* Working smarter and not making the CNC work harder. My prepared stock had two inches of extra height that needed to be removed to obtain the desired dimensions. At first, I generated a path that faced off this excess as a first step. When all other paths and setups were completed, I realized that this initial facing was taking a disproportionate amount of time. To fix this problem I used a bandsaw to cut the stock to a more appropriate size, showing me the power of thinking “outside the CNC”. 

