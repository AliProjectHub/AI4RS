# Change Detection with Modified CNNs on OSCD Dataset
## Overview
This repository contains code and resources for performing change detection using multiple modified Convolutional Neural Networks (CNNs) on the Onera Satellite Change Detection (OSCD) dataset. Change detection is a critical task in remote sensing, involving the identification of significant changes between satellite images taken at different times.

## Features
Implementation of several CNN architectures for change detection.
Modifications to standard CNNs to enhance performance on change detection tasks.
Preprocessing and augmentation techniques tailored for the OSCD dataset.
Evaluation metrics and visualization tools for assessing model performance.

## Usage


## Models
The repository includes implementations of several modified CNN architectures:

U-Net
FresU-Net
Modified U-Net (integrated Attention mechanism)
Each model can be configured and trained using the corresponding notebooks. Nevertheless this can become very time consuming therefore pretrained
 models and their weights are included
 
## Results
Performance of the models is evaluated using metrics such as:

- Precision
- Recall
- F1-Score
- Intersection over Union (IoU)
Results and model checkpoints are saved in the metrics and paths folders, respectively.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

# Acknowledgements
The OSCD dataset: OSCD Dataset
