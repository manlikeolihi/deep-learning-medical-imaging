
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

| Dataset Name | Modality | Size | # Cases | Description | Example Papers |
|--------------|----------|------|---------|-------------|----------------|
| [NIH Pancreas-CT](https://www.cancerimagingarchive.net/collection/pancreas-ct/) | CT | ~12 GB | 82 | Public dataset from NIH via TCIA, annotated for pancreas segmentation. Used widely for model benchmarking. | [U-Net (2015)](https://arxiv.org/abs/1505.04597), [Attention U-Net](https://paperswithcode.com/paper/attention-u-net-learning-where-to-look-for) |
| [MSD Task07: Pancreas](http://medicaldecathlon.com/) | CT | ~5 GB | 420 | Provided by MIC-DKFZ as part of the Medical Segmentation Decathlon (Task07). Labeled pancreas CT scans, benchmark dataset. | [nnUNet (2018)](https://arxiv.org/abs/1809.10486), [M3BUNet (2024)](https://arxiv.org/abs/2401.10419) |
| [BTCV (Beyond the Cranial Vault)](https://www.synapse.org/#!Synapse:syn3193805/wiki/217789) | CT | ~10 GB | 50 | Used in multi-organ segmentation tasks. Includes pancreas labels, used in challenges and deep learning papers. | [TransUNet (2021)](https://arxiv.org/abs/2102.04306), [Swin-Unet](https://arxiv.org/abs/2105.05537) |
| [AMOS 2022](https://amos22.grand-challenge.org/) | CT + MRI | ~180 GB | 500 | MICCAI 2022 abdominal segmentation challenge. Contains multiple organs including pancreas. | [AMOS 2022 Overview](https://amos22.grand-challenge.org/), [UCTransNet](https://paperswithcode.com/paper/uctransnet-rethinking-the-skip-connections-in) |

---


## External Dataset Links

- NIH Pancreas-CT: https://www.cancerimagingarchive.net/collection/pancreas-ct/
- MSD Task07: https://medicaldecathlon.com/
- BTCV: https://www.synapse.org/#!Synapse:syn3193805/wiki/217789
- AMOS 2022: https://amos22.grand-challenge.org/



These datasets are integral to the development and evaluation of deep learning models in medical image segmentation, particularly for pancreatic and abdominal imagin.

