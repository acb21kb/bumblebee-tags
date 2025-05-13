# Bumblebees: remote identification of individual bees using coloured retro-reflective tags

## Introduction
Understanding the flight paths and behaviours of bees is important for research into pollination patterns and monitoring ecosystems, making the ability to track behavioural patterns, such as foraging, a key area of research.

This project aims to identify individual bees by the colour of their tags using the retro-reflective tag and colour filter design, developed by Joyce [2] and Smith *et al.* [1]. The objective is to optimise the accuracy of colour detection and reduce misidentification.

Images of tags will be processed using a function that fits the tag data and generates a reconstruction. The pixel value error of this reconstruction will be minimised through an optimisation function and produce a more accurate estimate of the true filter colour of the tag, improving classification accuracy. Compared to the averaging method used by Joyce [2], this approach achieved an increase of 5.0% accuracy for 40 tag colours.

Increasing the number of distinguishable tag colours and achieving higher classification accuracy will allow more bees to be tracked simultaneously, allowing researchers to use multiple bees and substantially increase throughput of behavioural experiments.

The main objective is to assess whether a more accurate estimate of the tag colour could be produced by using the increased pixel coverage of the tag reflection when captured out-of-focus, coupled with an optimisation function to minimise pixel value error.

## Description
Methods and approaches to researching a solution to this project were developed in [development_code.ipynb](development_code.ipynb), with the final streamlined code saved in [full_implementation.ipynb](full_implementation.ipynb).

The fitted values of all tags in the dataset were saved in [all_tag_predictions.pkl](all_tag_predictions.pkl) for more time efficient processing.

## Conclusion
Overall, this approach resulted in a more accurate tag colour detections, enabling better tag classification. With further work and supplementary testing, this method could be developed to a workable addition to the retro-reflective tracking system developed by Smith *et al.* [1] and Joyce [2].

## Contributors
Author - Katie Broadhurst <kbroadhurst1@gmail.com>

Supervisor - Michael Smith <m.t.smith@sheffield.ac.uk>

## References
[1] M. T. Smith, M. Livingstone, and R. Comont, “A method for low-cost,
low-impact insect tracking using retroreflective tags,” Methods in Ecology and Evolution, vol. 12, no. 11, pp. 2184–2195, 2021. doi: https://doi.org/10.1111/2041-210X.13699. [Online]. Available: https://besjournals.onlinelibrary.wiley.com/doi/abs/10.1111/2041-210X.13699

[2] L. Joyce, “Differentiating bees using coloured retro-reflective tags,” M.S.
thesis, University of Sheffield, 2023.
