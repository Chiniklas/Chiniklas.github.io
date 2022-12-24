---
layout: default
title: "Lecture Project: Tour into the picture"
date: 2022-08-01
category: projects
image: /images/display_images/Tour into the picture.gif
authors: "<strong>Chi Zhang</strong>"
advisor: "Martin Kleinsteuber"
venue: "Grade 1.3"
# slides: research/pdf/ddp_presentation.pdf
# report: /research/pdf/DDP_report.pdf
code: https://github.com/Chiniklas/Computer-Vision-challenge.git
---
In this project we provide an interactive application, which enables the user to generate animation from a single 2D image. This application provides users with the following functions in the form of GUI: select an image, select the foreground object, select the vanishing point and inner rectangle, as well as change the perspective. <br><br>
Firstly, once the user has selected foreground objects, it's possible to distinguish foreground objects from background. Secondly, the user adds vanishing point and inner rectangle (rear wall) for the scene. Consequently, we can extract 5 regions from the picture. Based on the collection of polygons from background and foreground objects a simple scene model will be constructed.
