# Open Poetry Vision > 512x512
https://universe.roboflow.com/roboflow-gw7yv/open-poetry-vision

Provided by [Brad Dwyer](https://twitter.com/braddwyer)
License: CC BY 4.0

# Overview

The `Open Poetry Vision` dataset is a synthetic dataset created by Roboflow for OCR tasks.

It combines a random image from the [Open Images Dataset](https://storage.googleapis.com/openimages/web/index.html) with text primarily sampled from [Gwern's GPT-2 Poetry project](https://www.gwern.net/GPT-2). Each image in the dataset contains between 1 and 5 strings in a variety of fonts and colors randomly positioned in the 512x512 canvas. The classes correspond to the font of the text.

Example Image:
![Example Image](https://i.imgur.com/sZT516a.png)

# Use Cases

A common OCR workflow is to use a neural network to isolate text for input into traditional optical character recognition software. This dataset could make a good starting point for an OCR project like business card parsing or automated paper form-processing.

Alternatively, you could try your hand using this as a neural font identification dataset. Nvidia, amongst others, have [had success with this task](https://news.developer.nvidia.com/font-identification-from-real-world-images/).

# Using this Dataset

Use the `fork` button to copy this dataset to your own Roboflow account and export it with new preprocessing settings (perhaps resized for your model's desired format or converted to grayscale), or additional augmentations to make your model generalize better. This particular dataset would be very well suited for Roboflow's new advanced [Bounding Box Only Augmentations](https://blog.roboflow.ai/introducing-bounding-box-level-augmentations/).

## **Version 5 of this dataset (classes_all_text-raw-images)** has all classes remapped to be **labeled as "text."** This was accomplished by using [Modify Classes](https://docs.roboflow.com/image-transformations/image-preprocessing#modify-classes) as a [preprocessing step](https://docs.roboflow.com/image-transformations/image-preprocessing).

## **Version 6 of this dataset (classes_all_text-augmented-FAST)** has all classes remapped to be **labeled as "text."** and was trained with Roboflow's Fast Model.

## **Version 7 of this dataset (classes_all_text-augmented-ACCURATE)** has all classes remapped to be **labeled as "text."** and was trained with Roboflow's Accurate Model.
* [Introducing the New Roboflow Train](https://blog.roboflow.com/new-and-improved-roboflow-train/)
* [What to Think About When Choosing Model Sizes](https://blog.roboflow.com/computer-vision-model-tradeoff/)

# About Roboflow

[Roboflow](https://roboflow.ai) makes managing, preprocessing, augmenting, and versioning datasets for computer vision seamless.

Developers reduce 50% of their code when using Roboflow's workflow, automate annotation quality assurance, save training time, and increase model reproducibility.

#### [![Roboflow Workmark](https://i.imgur.com/WHFqYSJ.png =350x)](https://roboflow.ai)