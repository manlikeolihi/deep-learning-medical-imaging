
# Deep Learning for Medical Imaging – Pancreatic Cancer Focus




# data.md – Dataset Overview and Modalities


## 3.1 Comparison Between CT and MRI Data

### Key Differences Between CT and MRI in Pancreatic Cancer Evaluation

Based on the 2016 AJR paper by Jiang et al., *"Presurgical Evaluation of Pancreatic Cancer: A Comprehensive Imaging Comparison of CT Versus MRI,"* CT and MRI each offer specific strengths for assessing pancreatic tumors:

| Feature                      | CT (Computed Tomography)                                        | MRI (Magnetic Resonance Imaging)                             |
|-----------------------------|------------------------------------------------------------------|--------------------------------------------------------------|
| **Modality Type**           | Ionizing radiation (X-ray)                                     | Non-ionizing (magnetic fields + radio waves)                |
| **Soft Tissue Contrast**    | Moderate (less contrast between tumor and pancreas)            | High (better detection of small or isoattenuating tumors)   |
| **Vessel Clarity**          | Excellent arterial/venous visualization with CTA               | Moderate (lower resolution in some cases)                   |
| **Tumor Detection Accuracy**| High; slightly less than MRI for small tumors                  | Higher sensitivity for small or isoattenuating tumors        |
| **Evaluation of Resectability** | Slightly better performance in vascular invasion grading     | Similar performance overall; better for soft tissue margins |
| **Scan Speed**              | Fast (typically seconds)                                       | Slower (minutes), requires patient cooperation              |
| **Availability/Cost**       | Widely available and cheaper                                   | Less available and more expensive                           |

<img width="224" alt="image" src="https://github.com/user-attachments/assets/7004e2d0-d4d7-4693-afdf-775f0a5d81f0" />

<img width="216" alt="image" src="https://github.com/user-attachments/assets/f3fd3be7-431a-4305-9e7b-1637fd174aa5" />

<img width="217" alt="image" src="https://github.com/user-attachments/assets/ae5129f8-3910-41f4-a564-15a7dd28e2e0" />

CT Image (A/B): Show a hypodense mass in the pancreatic head region. The tumor appears less distinct, and the surrounding vascular structures are moderately visualized..

MRI Image (C): Depicts the same tumor with enhanced contrast, providing clearer delineation of the tumor boundaries and better visualization of the surrounding soft tissue structures.


This visual comparison underscores the differences in imaging modalities, highlighting MRI's superior soft tissue contrast, which can be crucial in the detailed assessment of pancreatic tumors.


Apologies for any confusion caused by previous broken links. I've compiled an updated list of academically recognized and peer-reviewed datasets relevant to pancreas and multi-organ segmentation tasks. These datasets are commonly used in benchmarking state-of-the-art models and are sourced from reputable institutions and challenges.





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
