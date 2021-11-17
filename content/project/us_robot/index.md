---
title: Robotic Ultrasound Scanning for Human Leg
summary: Automatic scanning the vessels (net step - auto puncture)
tags:
- Computer vision
- Robot
date: "2021-06-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

**For this project, a paper is planed to write based on current result**

## Vessel detection
I developed a Real-time vessel and vessel wall detection (main for artery) with an U-Net structure Fully Convolution Network and vessel wall enhancement. The detection result can guide the movement of the robot.

![](./picture1.png)

![](./picture2.png)

The vessel detection result is shown below:

{{< video src="w.avi" controls="yes" >}}

## Robot Scanning

To make sure the contact between Ultrasound probe and the leg, the impendance control with a 6-axis force sensor is used for z-axis control.

To know wether the ultrasound image is usable, the iamge is calculated into confidence map to eveluate the qulity. Hence we can adjust the rotation of the probe to get a more confident (clear) image.

![](./confidence.png)

{{< video src="US.mp4" controls="yes" >}}