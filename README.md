
# Brain Tumor Segmentation with 3D MRI Scans

This project performs 3D segmentation of brain tumors, specifically gliomas, from MRI scans. It leverages MONAI, a deep learning framework tailored for healthcare imaging, as part of the BraTS 2021 challenge within the MICCAI competition. This segmentation pipeline aims to advance automated brain tumor analysis.

## Table of Contents
- [Brain Tumor Segmentation with 3D MRI Scans](#brain-tumor-segmentation-with-3d-mri-scans)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Dependencies](#dependencies)
  - [Task Description](#task-description)
  - [Usage](#usage)
  - [License](#license)

## Installation

To set up the environment, ensure you have Python installed, and then follow these steps:

```bash
# Install the required packages
pip install "monai-weekly[nibabel, tqdm]" matplotlib
```

## Dependencies

This project relies on several key libraries:

- **MONAI**: Medical Open Network for AI (for medical imaging)
- **Matplotlib**: Visualization of segmentation results
- **Torch**: PyTorch for neural network computations
- **TQDM**: Progress bar for data loading and model training

Ensure all dependencies are installed before running the notebook.

## Task Description

The goal of this notebook is to train and evaluate a 3D brain tumor segmentation model using MRI scans. Specifically, the notebook covers:

- **Dataset Preparation**: Loading and preprocessing MRI scans.
- **Model Definition**: Configuring a 3D segmentation model based on ResNet architecture.
- **Training**: Running a sliding window inference technique for model training.
- **Evaluation**: Using metrics like Dice Score to assess segmentation performance.

The segmentation targets three tumor regions: 
1. Whole Tumor
2. Tumor Core
3. Enhancing Tumor

This segmentation task is part of the larger **Brain Tumor Segmentation (BraTS) 2021 Challenge**.

## Usage

1. Clone this repository and navigate to the directory.
2. Run the notebook using Jupyter:

   ```bash
   jupyter notebook mri-brain-tumor-segmentation.ipynb
   ```

3. Follow each cell in sequence to set up, train, and evaluate the model.

> **Note**: You can specify a data directory with the `MONAI_DATA_DIRECTORY` environment variable to store results and reused downloads, or use a temporary directory as configured.

## License

This project is open-source and available under the MIT License.
