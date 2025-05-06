
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
# 📊 Pancreatic Cancer Segmentation Datasets

This document provides a curated list of publicly available datasets commonly used for pancreatic cancer segmentation tasks. Each entry includes a summary, modality, and real papers that used the dataset.

| Dataset Name | Modality | Sample Size | Description | Representative Papers |
|--------------|----------|-------------|-------------|-----------------------|
| [NIH Pancreas-CT](https://www.cancerimagingarchive.net/collection/pancreas-ct/) | CT | 82 patients | Abdominal CT scans with manual pancreas annotations. Widely used for pancreas segmentation tasks. | [Fixed-Point Model](https://paperswithcode.com/paper/a-fixed-point-model-for-pancreas-segmentation), [Recurrent Saliency Network](https://paperswithcode.com/paper/recurrent-saliency-transformation-network) |
| [MSD Task07 (Pancreas)](https://github.com/openmedlab/Awesome-Medical-Dataset/blob/main/resources/MSD_Pancreas_Tumour.md) | CT | 420 cases | Part of the Medical Segmentation Decathlon. Includes pancreas and tumor masks from 3D CT. | [DeformuX-Net](https://paperswithcode.com/paper/deformux-net-exploring-a-3d-foundation), [MiniGPT-Pancreas](https://paperswithcode.com/paper/minigpt-pancreas-multimodal-large-language) |
| [BTCV (Beyond the Cranial Vault)](https://www.synapse.org/#!Synapse:syn3193805/wiki/217789) | CT | 50 cases | Multi-organ abdominal CT dataset with segmentation labels, including the pancreas. | [UNETR](https://paperswithcode.com/paper/unetr-transformers-for-3d-medical-image), [DeepEdit](https://paperswithcode.com/paper/deepedit-deep-editable-learning-for) |
| [AMOS](https://amos22.grand-challenge.org/) | CT & MRI | 500 cases | Multi-organ segmentation benchmark across multiple hospitals. Includes pancreas masks. | [AMOS Benchmark](https://paperswithcode.com/paper/amos-a-large-scale-abdominal-multi-organ), [Efficient Context-Aware Network](https://paperswithcode.com/paper/efficient-context-aware-network-for-abdominal) |
| [Pancreatic-CT-CBCT-SEG](https://www.cancerimagingarchive.net/collection/pancreatic-ct-cbct-seg/) | CT & CBCT | 30 patients | CBCT-guided radiation therapy scans with expert organ-at-risk annotations. | [Nature Scientific Data (2022)](https://www.nature.com/articles/s41597-022-01758-9), [IEEE Access (2024)](https://ieeexplore.ieee.org/abstract/document/10912050) |
| [PanSegData (MRI Pancreas)](https://osf.io/kysnj/) | MRI | 767 scans (499 patients) | Largest annotated MRI pancreas dataset from 5 institutions. Aims to support generalization. | [Springer Chapter](https://link.springer.com/chapter/10.1007/978-3-030-60548-3_19), [ScienceDirect Study](https://www.sciencedirect.com/science/article/pii/S1424390321001101) |
| [pNETs Dataset](https://arxiv.org/abs/2501.17555) | CT | 469 patients | First dataset dedicated to Pancreatic Neuroendocrine Tumors. | [Segmentation Screening Study](https://paperswithcode.com/paper/segmentation-for-classification-of-screening), [Eur Radiol (2023)](https://link.springer.com/article/10.1007/s00330-023-10186-1) |
| [PCEUS Dataset](https://arxiv.org/abs/2409.04718) | Endoscopic Ultrasound (EUS) | 501 images | Endoscopic ultrasound dataset with pathologically confirmed labels. | [Nature Sci Rep (2021)](https://www.nature.com/articles/s41598-021-87748-0), [Cancer Journal (2023)](https://acsjournals.onlinelibrary.wiley.com/doi/full/10.1002/cncr.34772) |


