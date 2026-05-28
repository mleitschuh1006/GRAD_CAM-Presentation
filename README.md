# Grad-CAM Live Demonstration

This repository contains an interactive live demonstration based on the paper "Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization" (Selvaraju et al., 2017). 

The purpose of this project is to provide a practical illustration of how to interpret decisions made by Convolutional Neural Networks (CNNs) using gradient-based localization techniques.

## Features

* Pre-trained Model Integration: Utilizes a pre-trained ResNet50 model to classify images.
* Class Discrimination: Demonstrates the model's ability to isolate and focus on different target classes within the same image.
* Grad-CAM: Generates class-specific heatmaps to highlight the regions of the image that strongly influence the model's prediction.
* Guided Grad-CAM: Combines Grad-CAM with Guided Backpropagation to produce high-resolution, class-specific visualizations.

## Setup and Installation

This project uses uv for fast Python environment and dependency management.

1. Ensure uv is installed on your system.
2. Initialize the project and install the required dependencies by running the following command:

    uv add torch torchvision grad-cam opencv-python matplotlib requests numpy notebook

## Usage

The demonstration is structured as an interactive Jupyter Notebook. To start the environment, execute the following command in your terminal:

    uv run jupyter notebook

Once the Jupyter interface opens in your browser, navigate to the gradcam_demo.ipynb file and execute the cells sequentially to follow the demonstration.

## References

* Selvaraju, R. R., Cogswell, M., Das, A., Vedantam, R., Parikh, D., & Batra, D. (2017). Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization. Proceedings of the IEEE International Conference on Computer Vision (ICCV), 618-626. https://arxiv.org/abs/1610.02391
* Gildenblat, J. (2021). PyTorch library for CAM methods. GitHub repository. https://github.com/jacobgil/pytorch-grad-cam