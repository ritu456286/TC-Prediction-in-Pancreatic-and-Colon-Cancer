# Tumor Cellularity Prediction in Pancreatic and Colorectal Cancer

## Overview

This project focuses on predicting Tumor Cellularity (TC) in pancreatic and colorectal cancers using advanced deep learning techniques, particularly semantic segmentation. Tumor cellularity refers to the proportion of tumor cells within a tissue sample and plays a significant role in cancer diagnosis, treatment decisions, and prognosis.

The goal of this project is to accurately calculate tumor cellularity by segmenting the nuclei of tumor cells in histopathology images. By applying a U-Net architecture, the project aims to enhance the precision of tumor segmentation and facilitate the prediction of tumor cellularity in cancer tissues.

## Methodology

### Key Steps:

1. **Tumor Nucleus Segmentation:**
   - **U-Net Architecture**: The U-Net model is employed to perform semantic segmentation on histopathology images, distinguishing tumor cell nuclei from surrounding tissue.
   - **Watershed Algorithm**: The watershed algorithm is used to refine the segmentation and separate overlapping nuclei, providing more accurate nuclei count estimates.

2. **Nuclei Count:**
   - Post-segmentation, the total number of nuclei is counted, allowing for the determination of tumor cellularity within the tissue sample.

3. **Cellularity Calculation:**
   - Tumor cellularity is calculated by estimating the ratio of tumor cell nuclei to the total number of cells in the sample.

## Tech Stack

- **Python**
- **U-Net**: A convolutional neural network architecture designed for image segmentation.
- **Semantic Segmentation**: Applied to accurately segment the nuclei from histopathology images.
- **Nuclei Count**: Methods for counting tumor cell nuclei within the segmented images.
- **Watershed Algorithm**: A post-processing technique used to separate closely-packed nuclei.

## Results

The application of these methodologies provides an automated and accurate way to calculate tumor cellularity in pancreatic and colorectal cancer tissues, aiding in more effective clinical decision-making.

## Usage

1. Clone the repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the segmentation model on the histopathology dataset.
4. Obtain the segmented images and predicted tumor cellularity.

## Future Improvements

- Further enhancement of segmentation accuracy using additional post-processing techniques.
- Adding innovation to the Unet-Architecture.
- Expansion to other cancer types and datasets for a more generalized model.
- Implementation of additional metrics to assess model performance.
