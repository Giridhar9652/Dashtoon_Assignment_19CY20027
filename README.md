# Dashtoon_Assignment_19CY20027

# Neural Style Transfer with TensorFlow

## Overview

This notebook implements neural style transfer using TensorFlow, allowing users to blend the content of one image with the artistic style of another. The implemented algorithm optimizes the output image to match the content statistics of a content image and the style statistics of a style reference image.

## Table of Contents

1. [Introduction](#introduction)
2. [Setup](#setup)
    - [Dependencies](#dependencies)
    - [Notebook Execution](#notebook-execution)
3. [Usage](#usage)
    - [Input Images](#input-images)
    - [Visualizing Input](#visualizing-input)
    - [Style Transfer](#style-transfer)
4. [Customization](#customization)
    - [Adjusting Parameters](#adjusting-parameters)
    - [Handling Different Images](#handling-different-images)
5. [Limitations and Potential Improvements](#limitations-and-potential-improvements)

## Introduction

Neural style transfer is an optimization technique that blends the content of an image with the artistic style of another. This notebook uses a pre-trained model and TensorFlow to perform fast neural style transfer.

## Setup

### Dependencies

Before running the notebook, ensure you have the following dependencies installed:

- TensorFlow
- TensorFlow Hub
- NumPy
- Matplotlib
- Pillow (PIL)

You can install these dependencies using the following:

```bash
pip install tensorflow tensorflow-hub numpy matplotlib Pillow
```

### Notebook Execution

To run the notebook, use a Jupyter environment or Google Colab. Make sure to execute each cell sequentially.

## Usage

### Input Images

Specified the content and style images in the notebook. The content image represents the subject, and the style image provides the artistic style.

### Visualizing Input

The notebook includes functions to visualize the input images and their dimensions. Ensure the images are loaded correctly before proceeding.

### Style Transfer

Execute the style transfer cells to optimize the output image. Adjust the hyperparameters and experiment with different style and content layers.

## Customization

### Adjusting Parameters

Feel free to customize the style transfer process by adjusting parameters such as learning rate, total variation weight, style weight, and content weight.

### Handling Different Images

To use different images, modify the `content_path` and `style_path` variables with the URLs or file paths of your desired content and style images.

### Limitations:

1. **Fixed Style and Content Images:**
   - The code assumes fixed style and content images. If we want to generalize the code to handle different images dynamically, we would need to modify the code to accept user inputs or provide a mechanism for selecting images at runtime.

2. **Fixed Number of Epochs and Steps:**
   - The number of epochs and steps for optimization are fixed. For different style and content pairs, these values might need to be adjusted.

3. **Optimization Hyperparameters:**
   - Hyperparameters such as the learning rate, total variation weight, style weight, and content weight are set to fixed values. These values might need adjustment based on the specific use case or user preferences.

### Potential Improvements:

1. **Dynamic Image Size Handling:**
   - Adapting the code to handle images of different sizes dynamically would improve flexibility.
   - 
2. **Transfer Learning:**
   - Need to explore transfer learning techniques to fine-tune the model on a specific set of styles or content types could improve the quality of stylized images.


