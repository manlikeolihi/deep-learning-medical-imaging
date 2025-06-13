# Deep Learning for Medical Imaging  
## Pancreas Segmentation on CT using Segment Anything Model (SAM)

Author: Olihi Ikande Idikwu  
Supervisor: Zhangkai Wu  
Macquarie University, 2025

---

## Abstract

This project explores the zero-shot segmentation capability of Meta AI’s Segment Anything Model (SAM) in the context of medical imaging. Specifically, we evaluate SAM’s performance on pancreas segmentation using CT scans from the MSD Task07 dataset. SAM is applied without any fine-tuning or domain adaptation to assess its generalization capacity from natural images to clinical data. This investigation aims to identify SAM’s strengths and limitations in anatomical segmentation and lay the groundwork for future refinement modules.

---

## Table of Contents

- Dataset Overview
- Model Summary
- SAM Evaluation Pipeline
- Results
- How to Run
- References
- Weekly Consultation Meeting Log

---

## Dataset Overview

Further details are provided in `data.md`.

The primary dataset used in this study is MSD Task07 (Pancreas), which contains abdominal CT scans with pixel-wise organ annotations. It is sourced from the Medical Segmentation Decathlon and is publicly available for academic use.

| Dataset       | Modality | Target Organ | Annotation Type | Source                                                                 |
|---------------|----------|---------------|------------------|------------------------------------------------------------------------|
| MSD Task07    | CT       | Pancreas      | Pixel-level masks| https://www.synapse.org/#!Synapse:syn3193805/wiki/217789               |

---

## Model Summary

Detailed model architecture descriptions are available in `models.md`.

The Segment Anything Model (SAM) is a promptable image segmentation framework composed of three key components:
- A Vision Transformer (ViT) image encoder
- A prompt encoder for point, box, and mask inputs
- A lightweight mask decoder

SAM is trained on over one billion masks from natural images but is evaluated here in a zero-shot setting on clinical CT data. The goal is to assess its domain transferability without any retraining or adaptation.

---

## SAM Evaluation Pipeline

The full implementation is available in `sam_eval_pipeline.ipynb`.

This pipeline loads slice 55 from the CT scan `pancreas_005.nii.gz` in the MSD Task07 dataset. It then applies SAM using two types of prompts:
- A single point prompt placed manually at the center of the pancreas
- A bounding box prompt surrounding the organ region

The resulting segmentation masks are compared against the ground truth to evaluate spatial accuracy, anatomical alignment, and common failure modes. A pipeline diagram is also included under the `images/` folder for visual reference.

---

## Results

The segmentation results for slice 55 are summarized below. Visual comparisons are provided in the `results/` directory.

- `slice55_pointprompt.png`: Output mask generated from a single point prompt.
- `slice55_boxprompt.png`: Output mask generated from a bounding box prompt.
- `groundtruth_overlay.png`: Ground truth overlay of pancreas region on the CT slice.

Qualitative observations from these results informed the conclusions of Chapter 4 in the accompanying thesis document.

---

## How to Run

### Clone the Repository

```bash
git clone https://github.com/manlikeolihi/deep-learning-medical-imaging.git
cd deep-learning-medical-imaging

yo could replace my username with yours to run.

