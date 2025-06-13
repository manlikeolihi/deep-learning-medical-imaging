# Deep Learning for Medical Imaging  
## Pancreas Segmentation on CT using Segment Anything Model (SAM)

Author: Olihi Ikande Idikwu  
Supervisor: Zhangkai Wu  
Macquarie University, 2025



## Abstract

This project explores the zero-shot segmentation capability of Meta AI’s Segment Anything Model (SAM) in the context of medical imaging. Specifically, we evaluate SAM’s performance on pancreas segmentation using CT scans from the MSD Task07 dataset. SAM is applied without any fine-tuning or domain adaptation to assess its generalization capacity from natural images to clinical data. This investigation aims to identify SAM’s strengths and limitations in anatomical segmentation and lay the groundwork for future refinement modules.



## Table of Contents

- Dataset Overview
- Model Summary
- SAM Evaluation Pipeline
- Results
- How to Run
- References
- Weekly Consultation Meeting Log



## Dataset Overview

Further details are provided in `data.md`.

The primary dataset used in this study is MSD Task07 (Pancreas), which contains abdominal CT scans with pixel-wise organ annotations. It is sourced from the Medical Segmentation Decathlon and is publicly available for academic use.

| Dataset       | Modality | Target Organ | Annotation Type | Source                                                                 |
|---------------|----------|---------------|------------------|------------------------------------------------------------------------|
| MSD Task07    | CT       | Pancreas      | Pixel-level masks| https://www.synapse.org/#!Synapse:syn3193805/wiki/217789               |



## Model Summary

Detailed model architecture descriptions are available in `models.md`.

The Segment Anything Model (SAM) is a promptable image segmentation framework composed of three key components:
- A Vision Transformer (ViT) image encoder
- A prompt encoder for point, box, and mask inputs
- A lightweight mask decoder

SAM is trained on over one billion masks from natural images but is evaluated here in a zero-shot setting on clinical CT data. The goal is to assess its domain transferability without any retraining or adaptation.



## SAM Evaluation Pipeline

The full implementation is available in `sam_eval_pipeline.ipynb`.

This pipeline loads slice 55 from the CT scan `pancreas_005.nii.gz` in the MSD Task07 dataset. It then applies SAM using two types of prompts:
- A single point prompt placed manually at the center of the pancreas
- A bounding box prompt surrounding the organ region

The resulting segmentation masks are compared against the ground truth to evaluate spatial accuracy, anatomical alignment, and common failure modes. A pipeline diagram is also included under the `images/` folder for visual reference.



## Results

The segmentation results for slice 55 are summarized below. Visual comparisons are provided in the `results/` directory.

- `slice55_pointprompt.png`: Output mask generated from a single point prompt.
- `slice55_boxprompt.png`: Output mask generated from a bounding box prompt.
- `groundtruth_overlay.png`: Ground truth overlay of pancreas region on the CT slice.

Qualitative observations from these results informed the conclusions of Chapter 4 in the accompanying thesis document.



## How to Run

### Clone the Repository

```bash
git clone https://github.com/manlikeolihi/deep-learning-medical-imaging.git
cd deep-learning-medical-imaging

you could replace my username with yours to run.




## Weekly Consultation Meeting Log

This log documents the weekly meetings held between the student and supervisor throughout the course of the Thesis A project.

- **Week 4 (22 March 2025)**  
  The initial meeting was held to introduce the project theme and objectives. The student was assigned to explore the Segment Anything Model (SAM) and its potential applications in medical imaging. The MSD Task07 (pancreas) dataset was identified as a possible target.

- **Week 5 (28 March 2025)**  
  The scope was refined further, confirming the project would focus on evaluating SAM's zero-shot performance on pancreas segmentation using CT scans. Dataset download and early literature search began.

- **Week 6 (4 April 2025)**  
  Literature review was in progress. Technical understanding of SAM was discussed, including its architecture and prompt encoding mechanisms. A test pipeline using a single CT slice was proposed.

- **Week 7 (11 April 2025)**  
  The prompt-based segmentation concept was explored in more detail. The student was advised to prepare a pipeline using both point and box prompts on a well-defined CT slice to simplify evaluation.

- **Week 8 (18 April 2025)**  
  Ethics workshop week. A light check-in occurred, with no major technical updates.

- **Weeks 9–10 (Mid-semester Break)**  
  No formal consultation occurred during the scheduled semester break.

- **Week 11 (16 May 2025)**  
  Post-break catch-up. Supervisor reviewed the student’s preliminary literature review and clarified expected methodology structure. Work began on setting up the evaluation pipeline and refining research questions.

- **Week 12 (23 May 2025)**  
  No meeting was held this week, as the supervisor was attending an academic conference.

- **Week 13 (30 May 2025)**  
  Visual results were presented using SAM with point and box prompts on CT slice 55. Observations about segmentation quality and SAM’s anatomical limitations were discussed. Planning began for the thesis results and evaluation sections.

- **Week 14 (6–12 June 2025)**  
  Final review session. Focused on polishing the thesis, completing the GitHub repository, organizing result figures, and integrating references. Student confirmed readiness to submit Thesis A.




