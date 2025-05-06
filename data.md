
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





# 📊 Pancreatic Cancer Segmentation Datasets

This document provides a curated list of publicly available datasets commonly used for pancreatic cancer segmentation tasks. Each entry includes a brief summary, modality, sample size, and references to representative studies.

| Dataset Name | Modality | Sample Size | Description | Representative Papers |
|--------------|----------|-------------|-------------|-----------------------|
| [NIH Pancreas-CT](https://www.cancerimagingarchive.net/collection/pancreas-ct/) | CT | 82 patients | Abdominal CT scans with manual pancreas annotations. Widely used for pancreas segmentation tasks. | [Gibson et al., 2017](https://doi.org/10.1007/978-3-319-66179-7_28) |
| [MSD Task07 (Pancreas)](https://github.com/openmedlab/Awesome-Medical-Dataset/blob/main/resources/MSD_Pancreas_Tumour.md) | CT | 420 cases | Part of the Medical Segmentation Decathlon. Includes 3D CT images with pancreas and tumor annotations. | [Antonelli et al., 2022](https://doi.org/10.1038/s41597-022-01721-5) |
| [BTCV (Beyond the Cranial Vault)](https://www.synapse.org/#!Synapse:syn3193805/wiki/217789) | CT | 50 cases | Multi-organ abdominal CT dataset with manual segmentations, including the pancreas. | [Landman et al., 2015](https://doi.org/10.1007/978-3-319-24553-9_10) |
| [AMOS (Abdominal Multi-Organ Segmentation)](https://amos22.grand-challenge.org/) | CT & MRI | 500 cases | Large-scale dataset for multi-organ segmentation tasks, including the pancreas. | [Ji et al., 2022](https://doi.org/10.1007/978-3-031-16437-8_40) |
| [Pancreatic-CT-CBCT-SEG](https://www.cancerimagingarchive.net/collection/pancreatic-ct-cbct-seg/) | CT & CBCT | 30 patients | Focused on CBCT-guided radiation therapy with physician-drawn segmentations of organs at risk. | [TCIA, 2022](https://doi.org/10.7937/TCIA.2022.1O1Y8F6G) |
| [PanSegData (MRI Pancreas Dataset)](https://osf.io/kysnj/) | MRI | 767 scans from 499 participants | Largest publicly available MRI pancreas dataset, collected from five centers. | [Bagci et al., 2023](https://github.com/NUBagciLab/PANSegNet) |
| [pNETs Dataset](https://arxiv.org/abs/2501.17555) | CT | 469 patients | First dataset dedicated to Pancreatic Neuroendocrine Tumors (pNETs) with contrast-enhanced CT images. | [Li et al., 2025](https://arxiv.org/abs/2501.17555) |
| [PCEUS Dataset](https://arxiv.org/abs/2409.04718) | EUS | 501 images | Pancreatic Cancer Endoscopic Ultrasound dataset with pathologically confirmed images. | [Yan et al., 2024](https://arxiv.org/abs/2409.04718) |
