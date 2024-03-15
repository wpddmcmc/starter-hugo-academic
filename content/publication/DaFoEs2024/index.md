---
title: "DaFoEs: Mixing Datasets Towards the Generalization of Vision-State Deep-Learning Force Estimation in Minimally Invasive Robotic Surgery"
authors:
- Mikel De Iturrate Reyzabal
- admin
- Wei Huang
- Sebastien Ourselin
- Hongbin Liu
# author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2024-01-22T00:00:00Z"
doi: "10.1109/LRA.2024.3356984"

# Schedule page publish date (NOT publication's date).
publishDate: "2024-01-22T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "IEEE Robotics and Automation Letters"
publication_short: ""

abstract: Precisely determining the contact force during safe interaction in Minimally Invasive Robotic Surgery (MIRS) is still an open research challenge. Inspired by post-operative qualitative analysis from surgical videos, the use of cross-modality data driven deep neural network models has been one of the newest approaches to predict sensorless force trends. However, these methods required for large and variable datasets which are not currently available. In this paper, we present a new vision-haptic dataset (DaFoEs) with variable soft environments for the training of deep neural models. In order to reduce the bias from a single dataset, we present a pipeline to generalize different vision and state data inputs for mixed dataset training, using a previously validated dataset with different setup. Finally, we present a variable encoder-decoder architecture to predict the forces done by the laparoscopic tool using single input or sequence of inputs. For input sequence, we use a recurrent decoder, named with the prefix R, and a new temporal sampling to represent the acceleration of the tool. During our training, we demonstrate that single dataset training tends to overfit to the training data domain, but has difficulties on translating the results across new domains. However, dataset mixing presents a good translation with a mean relative estimated force error of 5% and 12% for the recurrent and non-recurrent models respectively. Our method, also marginally increase the effectiveness of transformers for force estimation up to a maximum of ≃15% , as the volume of available data is increase by 150%. In conclusion, we demonstrate that mixing experimental set ups for vision-state force estimation in MIRS is a possible approach towards the general solution of the problem.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'featured.gif'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

