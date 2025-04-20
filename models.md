

## models/model_collection.md

###  Deep Learning Models for Pancreatic Cancer

# Model Summaries

This document summarizes recent models used for medical image segmentation, focusing on pancreatic cancer and abdominal organs.

| Model Name | Venue (Year) | Backbone | Machine Learning Task | Segmentation Task | Device |
|:-----------|:-------------|:---------|:----------------------|:------------------|:-------|
| TransUNet | MICCAI 2021 | Transformer + U-Net | Transformer-based segmentation | Abdominal organ segmentation (including pancreas) | Tesla V100 |
| TransFuse | MICCAI 2021 | CNN + Transformer Fusion | Hybrid feature segmentation | General medical segmentation (applicable to pancreas) | RTX 3090 |
| CoTr | MICCAI 2021 | CNN + Transformer | 3D medical segmentation | Multi-organ CT segmentation (includes pancreas) | Tesla V100 |
| UNETR | WACV 2022 | Transformer Encoder + U-Net Decoder | Volumetric segmentation | Multi-organ CT/MRI segmentation | Tesla V100 |
| nnFormer | CVPR 2022 / TIP 2023 | Transformer | 3D medical segmentation | Multi-organ 3D segmentation (CT/MRI, pancreas included) | RTX 3090 |
| Swin-Unet | ECCV Workshop 2022 | Swin Transformer | Pure transformer segmentation | Multi-organ CT/MRI segmentation | A100 GPU |
| Medical Transformer (MedT) | MICCAI 2021 | Gated Axial Transformer | Segmentation with small datasets | Medical image segmentation (good for low-data tasks like pancreas) | GTX 1080Ti |
| DiNTS | CVPR 2021 | NAS-discovered CNN | Neural Architecture Search segmentation | Pancreatic tumor segmentation (Medical Segmentation Decathlon) | RTX 3090 |
| nnU-Net | Nature Methods 2021 | Self-configuring U-Net | AutoML segmentation | Pancreatic tumor segmentation (NIH, MSD) | V100 |
| Swin UNETR | MICCAI 2022 | Swin Transformer | 3D semantic segmentation | Brain tumor and general organ segmentation (transferable to pancreas) | A100 GPU |

