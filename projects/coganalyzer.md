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

Here's some code to demonstrate what the program did:

# COG file used
cog_file = 'f.tif'

# Open the COG file in read mode
with rasterio.open(cog_file) as dataset:
    # Get the dimensions of the image tiles
    tile_width, tile_height = dataset.block_shapes[0]

    # Loop through each tile in the dataset
    for x in range(0, dataset.height, tile_height):
        for y in range(0, dataset.width, tile_width):
            # Calculate the pixel coordinates of the current tile
            target_tile_window = ((x, x + tile_height), (y, y + tile_width))

            # Read the data of the current tile
            tile_data = dataset.read(window=target_tile_window)

            # Create a PIL image from the tile_data (assuming it has 3 bands, e.g., RGB)
            tile_image = Image.fromarray(tile_data.transpose(1, 2, 0))

            # Save the tile image with a specific name or index
            # tile_image_path = f'tile_{x}_{y}.png'
            # tile_image.save(tile_image_path)

            # Show image, histogram, and print tile data
            tile_image.show()
            show_hist(tile_data, bins=50, histtype='stepfilled', lw=0.0, stacked=False, alpha=0.3)
            print(tile_data)
