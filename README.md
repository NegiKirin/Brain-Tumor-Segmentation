# Brain Tumor Segmentation

This repository implements a comparative analysis of deep learning models (UNet, ResUNet, DeepResUNet, DRU, SRU, DuckNet) for brain tumor segmentation, as per the paper by Quang-Huyen Tran et al. from The University of Da Nang - University of Science and Technology, Vietnam.

## Dataset
- Source: [Figshare](https://figshare.com/articles/dataset/brain_tumor_dataset/1512427)
- Details: 3,064 MRI image-mask pairs (512×512 pixels, grayscale with binary masks).

## Usage
- Run notebooks in `notebooks/` for model training and evaluation.

## Models
- UNet, ResUNet, DeepResUNet, DRU, SRU, DuckNet.

## Results
| Model         | Parameters | Train Dice | Train IoU  | Test Dice  | Test IoU   |
|---------------|------------|------------|------------|------------|------------|
| UNet          | 31.3M      | **0.9833** | 0.9577     | 0.8050     | 0.7232     |
| ResUNet       | 31.5M      | **0.9833** | **0.9674** | 0.8062     | 0.7233     |
| DeepResUNet   | 32.6M      | 0.9792     | 0.9597     | 0.8047     | 0.7235     |
| DRU           | 13.9M      | 0.9065     | 0.8301     | 0.7954     | 0.6699     |
| SRU           | **12.7M**  | 0.9260     | 0.8630     | 0.7825     | 0.6561     |
| DuckNet       | 38M        | 0.9753     | 0.9520     | **0.8575** | **0.7561** |