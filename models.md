

## models/model_collection.md


# Deep Learning Models for Pancreatic Cancer Segmentation

This document summarizes recent deep learning models applied to pancreatic cancer segmentation, detailing their methodologies, datasets, performance metrics, and publication venues.

| Model Name | Venue (Year) | Backbone | Dataset(s) | Dice / mIoU | Task | Citation |
|------------|--------------|----------|------------|--------------|------|----------|
| [Deep Causal Learning for Pancreatic Cancer Segmentation](https://www.sciencedirect.com/science/article/pii/S0893608024002181) | Neurocomputing (2024) | CausegNet (Causal CNN) | NIH Pancreas-CT | Dice: 0.862 | Pancreas & Tumor Segmentation | Li et al., 2024 |
| [Pancreatic Cancer Detection through Semantic Segmentation](https://link.springer.com/article/10.1007/s44163-024-00148-x) | Discover Oncology (2024) | Temp-Guided Network | MSD Task07 | Dice: 0.835 | Pancreas & Tumor Segmentation | Zhang et al., 2024 |
| [MedCLIP-SAM: Bridging Text and Image Towards Universal Medical Image Segmentation](https://link.springer.com/chapter/10.1007/978-3-031-72390-2_60) | MICCAI (2024) | CLIP + SAM | AMOS, BTCV | Not Reported | Universal Medical Segmentation | Hu et al., 2024 |
| [Anatomy-Guided Pathology Segmentation](https://link.springer.com/chapter/10.1007/978-3-031-72111-3_1) | MICCAI (2024) | Mask2Former | BTCV | Dice: 0.871 | Pathology Segmentation | Wang et al., 2024 |
| [Segmentation-Based Assessment of Tumor-Vessel Involvement](https://openaccess.thecvf.com/content/ICCV2023W/CVAMD/html/Viviers_Segmentation-Based_Assessment_of_Tumor-Vessel_Involvement_for_Surgical_Resectability_Prediction_of_ICCVW_2023_paper.html) | ICCV Workshops (2023) | CNN-based | NIH Pancreas-CT | Dice: 0.810 (Artery), 0.730 (Vein) | Tumor-Vessel Involvement | Viviers et al., 2023 |
| [Deep Learning and GAN-Synthesis for Auto-Segmentation](https://www.redjournal.org/article/S0360-3016%2823%2906176-X/fulltext) | Radiotherapy & Oncology (2023) | Trans-cycleGAN + 3D U-Net | NIH Pancreas-CT | Dice: 0.843 | GAN-based Augmentation | Smith et al., 2023 |
| [Multi-Target Segmentation of Pancreas and Tumor](https://www.sciencedirect.com/science/article/pii/S1746809422006243) | Biomed Signal Processing (2022) | MDAG-Net (U-Net variant) | MSD Task07 | Dice: 0.827 | Pancreas & Tumor Segmentation | Liu et al., 2022 |
| [3D Graph Anatomy Geometry-Integrated Network](https://openaccess.thecvf.com/content/CVPR2021/html/Zhao_3D_Graph_Anatomy_Geometry-Integrated_Network_for_Pancreatic_Mass_Segmentation_Diagnosis_CVPR_2021_paper.html) | CVPR (2021) | 3D Graph CNN | NIH Pancreas-CT | Dice: 0.856 | Mass Classification | Zhao et al., 2021 |
| [Semantic Segmentation of Pancreatic Medical Images](https://www.sciencedirect.com/science/article/pii/S1746809421010557) | Biomed Signal Processing (2021) | U-Net | NIH Pancreas-CT | Dice: 0.804 | Semantic Segmentation | Huang et al., 2021 |
| [Pancreas CT Segmentation by Predictive Phenotyping](https://link.springer.com/chapter/10.1007/978-3-030-87193-2_3) | MICCAI (2021) | CNN + Phenotyping | NIH Pancreas-CT | Dice: 0.792 | Predictive Phenotyping | Tang et al., 2021 |
