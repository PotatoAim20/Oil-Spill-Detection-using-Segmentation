# Oil Spill Detection Using Segmentation

This repository contains code and data for detecting oil spills in SAR images using segmentation techniques. The project utilizes three different models: U-Net, DeepLabV3, and PSPNet, to achieve accurate segmentation.

## Data

The dataset is split into training and testing sets:

- **Training set**: 1002 samples
- **Testing set**: 110 samples

Each set contains three folders:
- **images**: SAR images in .jpg format
- **labels**: Ground truth segmentation RGB masks in .png format

### RGB Masks

The segmentation masks use the following color codes to represent different classes:

- **Black**: Sea Surface
- **Cyan**: Oil Spill
- **Red**: Look-alike
- **Brown**: Ship
- **Green**: Land

### RGB Values

The RGB values for each class are as follows:

- **Black**: (0, 0, 0)
- **Cyan**: (0, 255, 255)
- **Red**: (255, 0, 0)
- **Brown**: (153, 76, 0)
- **Green**: (0, 153, 0)

## Models

Three different models were used for segmentation:

1. **U-Net**: A convolutional network for biomedical image segmentation.
2. **DeepLabV3**: An atrous convolutional network for semantic image segmentation.
3. **PSPNet**: Pyramid Scene Parsing Network for pixel-wise semantic segmentation.

- [U-Net](https://arxiv.org/abs/1505.04597)
- [DeepLabV3](https://arxiv.org/abs/1706.05587)
- [PSPNet](https://arxiv.org/abs/1612.01105)
