# Advanced Image Processing Pipeline for Object Detection with FloodNet Dataset

## Introduction

Prepare Dataset is an innovative image processing pipeline designed to facilitate the preparation of datasets for deep learning applications in object detection and segmentation, with a special focus on handling `FloodNet` dataset masks. This project streamlines the conversion of FloodNet's detailed segmentation masks into YOLO format, ensuring datasets are optimally prepared for training high-precision object detection models.

## Motivation

The motivation behind this project stems from the challenges faced during the dataset preparation phase in computer vision tasks. Properly formatted and processed datasets are crucial for training accurate and efficient models. This project addresses these challenges by providing a comprehensive pipeline that automates the tedious aspects of dataset preparation, allowing researchers and developers to focus on model development and experimentation.



## Core Technologies and Techniques

This project utilizes a variety of image processing libraries and techniques to accomplish its goals. Key among these are OpenCV for image manipulation, NumPy for efficient numerical computations, and Matplotlib for visualization purposes. The pipeline leverages these tools to perform tasks such as resizing images, converting image formats, and visualizing object detection results with precision.

### Predefined Functions Overview

1. **Environment Setup Functions**: Automate the setup of the necessary environment, ensuring that all dependencies are correctly installed and configured.

2. **Image Resizing Functions**: Utilize OpenCV to resize images according to the input requirements of various object detection models, maintaining aspect ratio and image quality.

3. **Segmentation Mask Conversion**: Convert segmentation masks into YOLO format using predefined functions that parse and transform mask data, ensuring compatibility with YOLO's object detection framework.

4. **YOLO Label Generation**: Generate labels in YOLO format, accurately reflecting the position and class of each object in the image, facilitating efficient model training.

5. **Class-specific Box Drawing**: Implement custom functions to draw bounding boxes around detected objects, using class-specific colors to enhance the clarity and utility of visualized results.

6. **Visualization Tools**: Deploy Matplotlib-based functions for the graphical representation of object detection outcomes, allowing for immediate visual feedback and adjustment.

## Methodologies

### Image Resizing and Saving

Resizing images for object detection tasks is crucial to standardize input size for models and improve computational efficiency. This pipeline employs interpolation techniques to resize images without significant loss of detail, preserving the integrity of the original data for accurate object detection.

### Converting Segmentation Masks to YOLO Format

The conversion process involves analyzing segmentation masks, identifying object boundaries, and translating this information into the YOLO format. This includes calculating the center points, width, and height of bounding boxes in a normalized form, enabling seamless integration with YOLO-based object detection models.

### Visualization of Detection Results

Visual feedback is essential for the iterative process of model training and tuning. The visualization tools developed for this project allow users to overlay bounding boxes on images, directly observe the performance of object detection models, and make necessary adjustments to parameters or preprocessing steps.

### FloodNet Dataset Masks

The [**FloodNet dataset**](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021?fbclid=IwAR2XIwe5nJg5VSgxgCldM7K0HPtVsDxB0fjd8cJJZfz6WMe3g0Pxg2W3PlE) is a comprehensive collection of images and segmentation masks designed for flood detection and analysis.

## Installation

### Prerequisites

- Python 3.x
- Jupyter Notebook
- OpenCV
- NumPy
- Matplotlib

### Setup

Clone the repository and navigate to the project directory:

```bash
git clone [Repository-URL]
cd [Project-Directory]
```

Launch Jupyter Notebook and open the `From masks to bounding boxes for YOLO.ipynb` file:

```bash
jupyter notebook
```

## Contributing

We welcome contributions from the community! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## Usage

Follow the step-by-step instructions within the Jupyter notebook `Prepare_Dataset_V_01.ipynb`. Each section is designed to guide you through different phases of dataset preparation, from initial setup to visualization of results.

### Examples

```python
# Example of resizing an image
resize_image('path/to/image.jpg', output_size=(416, 416))

# Example of converting a segmentation mask to YOLO format
convert_mask_to_yolo('path/to/mask.jpg', 'path/to/output.txt')

# Example of visualizing detection results
draw_boxes_with_labels('path/to/image.jpg', 'path/to/detection_results.txt', 'path/to/output_path/annotated_image.jpg')
```

## Authors
- [**ABDELKADIR Sellahi**](https://github.com/AbdelkadirSellahi)
