---
title: Visual Servoing for Flexible Endoscopic Robot
summary: MSc Final Project (Mark:88/100)
tags:
- Computer vision
- Robot
date: "2020-03-20T00:00:00Z"

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
url_code: ""
url_pdf: "./MingcongChen_19007740_HongbinLiu_FinalReport_2019-20.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---
[View my master degree theisis <i class="fas fa-file-pdf"></i>](./MingcongChen_19007740_HongbinLiu_FinalReport_2019-20.pdf)

The flexible endoscopic robot has shown great potential in minimally invasive surgery. Compared with conventional open surgery, The endoscopic robot will cause less pain and lower bleeding rates which can help patients recover faster. However, the current endoscopic robot system relies on the surgeon too much that will lead to the lack of surgeon resources and cause danger when the surgeon is getting tired after long-duration operations. Moreover, with the development of 5G, the discussion about the benefit of remote surgery has been revealed to the public. Especially in today's medical situation, due to the coronavirus, the remote surgical system becomes more and more important. At present, there are already several soft manipulators based on cable drive that has been developed, which allows an accurate movement and force control resulting in safety risk for the patient. To give a more straightforward model for the robot, a helix mesh design of the robot’s tip is investigated in this project. A cable-driven actuation system is also developed with a Wi-Fi-based remote controller system. To realize accurate control, the soft robot in this project is modeled by constant curvature to set up the relationship between working space, joint space, and actuator space. Moreover, an inverse kinematics model can solve the visual servoing task is demonstrated based on the differential Jacobian matrix and the estimated Jacobian matrix. All the algorithms are tested in a simulated experiment, and a physical robot experiment for target guided controlling, which shows the desired stable movement. Furthermore, the visual servoing of the soft robot is validated using a painted target showing adequately accurate movement and linear behavior. As an inspiration result, an external contact location estimation algorithm is discussed by an experiment based on visual servoing.The expected work in the future is the combination with a haptic sensor on the tip of the robot 
to give a duel-feedback control and the hyper-remote control based on a 5G modular.
{{< video src="robot.mp4" controls="yes" >}}
with calculated Jacobia
{{< video src="servo1.mp4" controls="yes" >}}
with estimated Jacobia
{{< video src="servo2.mp4" controls="yes" >}}
## Robot System Design
Soft Robot
MicroDART is a multi-DOF flexible endoscopic robot. The robot’s hardware contains six main parts, including catheter, camera, multi-channel tube, tendons, actuators, and control box. The catheter is a high-performance nylon 3-D printed structure that can provide the robot bending ability. Tendon is a steel wireline used to pass through the multi-channel tube which connected with the catheter to control the bending angle. Five stepper motors linked to screw platforms act as actuators for the system. Motor drivers and controllers with Wi-Fi modular are located in the control box.
![ee](./robot.png)

![ee](./force.png)

![ee](./1.png)
The control algorithm of the robot is image-guided feedback control. At first, to control the robot, a forward kinematics model called constant curvature is introduced, which can set up the relationship among end-effector working space, joint space, and driven space. PC can recognize the catheter tip position and target position by real-time video stream, in which the position error in the image can be calculated. As well as the error from image inputs into aninverse kinematics method based on the Jacobian matrix and target error to get the joints to pose. During the movement, the Jacobian matrix will keep updating until the robot reaches the target and stop moving.
## Result
In simulated trajectory, the visual servoing algrithom can follow the target well.

![](./jm.png)

In real world robot, the robot tip trajectory and the simulated target

![](./ejm.png)

There is a target put in front of the robot with different positions. All three trajectories can coverage under the visual servoing algorithm. However, the trajectory still shows some oscillation during the movement which caused the trajectory was not the shortest path from the start point to the end point. As table 3.1 shown, each target is tested ten times and the iteration times are both from 13 to 22 that means iteration speed is not related to the target distance

![](./vs.png)