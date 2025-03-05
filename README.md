# Bumblebees: remote identification of individual bees using coloured retro-reflective tags

## Introduction
The ability to track bee behaviour is extremely important in understanding the inner workings of bee colonies and how they interact with the environment. Bees play an essential role in pollination and monitoring the activity of
individual bees can allow for a more in depth view of the effects that changes in the environment can produce, such as pesticides or climate change.

This project aims to aid in the tracking of bees in their natural environment without the tracking system disrupting their behaviour, by developing an effective method of identifying individual bees using a camera set up and small retro-reflective tags with coloured light filters to give each tag a unique
colour. Previous research [1] [2] developed a lightweight and low cost approach using these tags. The process uses consecutive images captured with and without flash, aligning them and then subtracting the no-flash image to find the brightest spot which should be the location of the tag in the image.

Due to the photos being captured in an outdoor environment there will be other reflections that are also picked up on camera. To decrease these false
positives, any reflections that are stationary between photos are removed. As well as this, a machine learning algorithm was developed to identify any
non-stationary reflections that are larger than a pixel, as the reflections from the bee tags are expected to be smaller than this measure, and only consider
the reflections that remain.

As it is expected to appear as less than a pixel, the processing needed to detect tag colours will need to take into account the colour interference
from the camera’s Bayer filter. A Bayer filter is an alternating pattern of red, green and blue pixels that overlays the photo captured by the camera
and would slightly alter the appearance of the reflection when smaller than a single pixel.

## Description
Methods and approaches to developing a solution to this project will be developed here.

## Contributors
Author - Katie Broadhurst <kbroadhurst1@gmail.com>

Supervisor - Michael Smith <m.t.smith@sheffield.ac.uk>

## References
[1] M. T. Smith, M. Livingstone, and R. Comont, “A method for low-cost,
low-impact insect tracking using retroreflective tags,” Methods in Ecology and Evolution, vol. 12, no. 11, pp. 2184–2195, 2021. doi: https://doi.org/10.1111/2041-210X.13699. [Online]. Available: https://besjournals.onlinelibrary.wiley.com/doi/abs/10.1111/2041-210X.13699

[2] L. Joyce, “Differentiating bees using coloured retro-reflective tags,” M.S.
thesis, University of Sheffield, 2023.
