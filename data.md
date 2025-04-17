
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



###  Dataset Summary Table
| Dataset Name                                | Modality | Data Size | # of Samples | Image Size         | Notes                                                                  |
|---------------------------------------------|----------|-----------|--------------|--------------------|------------------------------------------------------------------------|
| BTCV (Beyond the Cranial Vault)             | CT       | ~10 GB    | 50           | 512×512×N slices   | Used in TransUNet, CoTr, UNETR, Swin-Unet                              |
| MSD Task07: Pancreas (Medical Decathlon)    | CT       | ~5 GB     | 420          | 512×512×N slices   | Benchmark for nnU-Net, DiNTS, and other top models                     |
| NIH Pancreas-CT Dataset                     | CT       | ~12 GB    | 82           | Varies             | NIH-based, peer-reviewed, used in nnU-Net comparison studies           |
| BraTS 2021 (Brain Tumor Segmentation)       | MRI      | ~200 GB   | ~2000        | 240×240×155 voxels | Used in Swin-UNETR, MedT — benchmark for MRI segmentation              |
| AMOS 2022 (Abdominal Multi-organ Segmentation) | CT + MRI | ~180 GB   | 500 (mix)     | 512×512×N slices   | Recent MICCAI challenge used in hybrid model evaluation                |


### External Dataset Links

- **BTCV** [Zenodo - BTCV Dataset](https://zenodo.org/record/116936)
- **MSD Task07** [Medical Segmentation Decathlon](http://medicaldecathlon.com)
- **NIH Pancreas-CT** [The Cancer Imaging Archive - Pancreas-CT](https://www.cancerimagingarchive.net/collection/pancreas-ct)
- **BraTS 2021** [RSNA-ASNR-MICCAI BraTS 2021 Challenge](https://www.med.upenn.edu/cbica/brats2021)
- **AMOS 2022** [AMOS 2022 Challenge](https://amos22.grand-challenge.org)

---
These datasets are integral to the development and evaluation of deep learning models in medical image segmentation, particularly for pancreatic and abdominal imagin.

