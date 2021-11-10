---
title: Lane detection and object detection 
summary: Inturn project in Inspur-Lane detection and object detection.
tags:
- Deep Learning
date: "2019-07-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/georgecushen
url_code: "https://github.com/wpddmcmc/lane_detection"
url_pdf: ""
url_slides: ""
url_video: "https://youtu.be/o-JSw9U2P-o"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

## Project finished by myself in Inspur, the main idea is simple:
### Binary image
Separate the channels and obtain three single channel gray images corresponding to blue, green and red respectively, Filter the values of each pixel of the three images respectively, for example, white Lane (b > 200, G > 200, R > 200, all set to 255, otherwise 0), Yellow Lane (b < 150, G > 200, R > 200, all set to 255, otherwise 0), Merge the images to obtain a three channel black-and-white binary image (only 255 and 0, i.e. 0 and 1).
### Perspective Transformation
Using the condition that the perspective center, image point and target point are collinear, according to the perspective rotation law, the background surface (perspective surface) rotates a certain angle around the trace (perspective axis), which destroys the original projection beam, and can still maintain the transformation of the projection geometry on the background surface.
### Sliding Windonws
### Least Square Method