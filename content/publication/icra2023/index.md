---
title: "Fully Robotized 3D Ultrasound Image Acquisition for Artery"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Mingcong Chen
- Yuanrui Huang 
- Jian Chen
- Tongxi Zhou
- Jiuan Chen  
- Hongbin Liu

# # Author notes (optional)
# author_notes:
# - "Equal contribution"
# - "Equal contribution"

date: "2023-05-29T00:00:00Z"
doi: "10.1109/ICRA48891.2023.10161148"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-05-29T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *2023 IEEE International Conference on Robotics and Automation*
publication_short: In *ICRA 2023*

abstract: Current imaging of the artery relies primarily on computed tomography angiography (CTA), which requires contrast injections and exposure to radiation. In this paper, we present a method for fully autonomous artery 3D image acquisition using a linear ultrasound (US) probe and a 6 DoFs robot arm with a 3D camera. Robotic vessel acquisition can minimize tissue deformation and permit the reproduction of scans. Additionally, the robotic-based acquisition can provide more precise vessel position data that can be utilized for 3D reconstruction as a preoperative image. The first scanning point is determined by the 3D camera using a neural network for leg area estimation. A visual servo algorithm adjusts the in-plane motions using a cross-sectional vessel segmentation produced by a neural network with a UNet structure, while a US confidence map regulates the in-plane rotation. The robot is equipped with impedance control to maintain a constant and safe scan. Experiments on a leg phantom and a volunteer indicate that the robot can follow the vessel and modify its position to provide a sharper US image. The average error of phantom scanning in y-axis and z-axis are 0.2536mm and 0.2928mm, respectively, while the root means square error (RMSE) of contact force in the volunteer experiment is 0.2664N. In addition, a 3D vessel reconstruction demonstrates the possibility of robotic US acquisition as a preoperative image.

# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

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
  caption: 'icra2023.png'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
# - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---
