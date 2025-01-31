---
layout: project
type: project
image: img/cotton/cotton-square.png
title: "Cloud GeoTIFF Analyzer"
date: 2023
published: true
labels:
  - Python
  - numpy
  - Rasterio
summary: "A program I developed to analyze GeoTIFF files while working at the Robotic Space Exploration Lab."
---

While doing my internship at the Robotic Space Exploration Lab at the University of Hawaii at Manoa, I was tasked with desiging a program that could extract data from a Cloud GeoTIFF (COG) file and generate a visual representation of the different properties of the terrain featured on the file. I was tasked this because the team I was working with was creating a rover to analyze terrain properties in different locations that could be saved as COGs to be analyzed, with the technology being used to eventually explore other planets. The unique feature of a COG is that is can store layers of data, called bands, that each represent a different characteristic of the geospacial image, with the color representing the value of the specific characteristic at any point on the image. To create this program, I decided to use the rasterio library in Python to open the file and separate it into individual tiles whos metadata could be analyzed and tagged to create a visual representation of the stored data in that tile that we were looking for.

This program went through many iterations, which taught me how to evolve programs to accomplish additional goals, as along the way of designing this program I was tasked to add certain features that I previously hadn't considered. My work on this program also helped me improve my research skills, as I initially had no idea what COGs were and how to analyze them, which led me to doing a lot of research in order to understand the pro work I had to do. Additionally, I wasn't given always given specific instructions as to what I was supposed to do, so I had to improve my ability to understand problems and come up with solutions for them on my own. Working on this project and internship overall helped me develop real world software engineering skills that I still use to this day.
