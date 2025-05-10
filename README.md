# Deep Learning for Medical Imaging – Pancreatic Cancer Segmentation

Welcome to the project repository for my research on applying deep learning techniques to medical imaging, with a focus on the detection and segmentation of pancreatic cancer.

This project investigates the use of prompt-based segmentation using Meta AI’s Segment Anything Model (SAM), evaluates key performance metrics, and reviews recent literature on deep learning models applied to medical imaging.

---

##  Project Overview

The goal of this research is to:
- Explore and evaluate deep learning techniques for segmenting pancreatic regions in CT and MRI scans
- Implement a segmentation pipeline using SAM with prompt types (point, box, automatic)
- Compare segmentation outputs using IoU, Dice Score, and Pixel Accuracy
- Curate datasets, models, and literature for future medical imaging work

This repository contains structured documentation, working code, and an end-to-end segmentation demonstration.

---

##  Repository Contents

| File/Folder | Description |
|-------------|-------------|
| `main_thesis.md` | Complete thesis document with all section links |
| `environment_setup.md` | Python environment and library setup |
| `experiments.md` | Experimental design, metrics, and results |
| `models.md` | Summary of deep learning models and architectures used |
| `literature_review.md` | Key papers from CVPR, MICCAI, ECCV, etc. |
| `data.md` | CT vs MRI comparison and dataset summaries |
| `TOYEXAMPLE_UPDATED_ANNOTATED.ipynb` | Notebook demonstrating segmentation using SAM |
| `docs/` | Diagrams, sample outputs, and images (if applicable) |
| `papers/` | Curated academic papers for reference |
| `datasets/` | Dataset links and summaries |
| `scripts/` | (To be added) Scripts for training, evaluation, and preprocessing |

---

##  Sample Results

| Prompt Type       | IoU   | Dice Score | Pixel Accuracy |
|-------------------|-------|------------|----------------|
| Point Prompt      | 0.64  | 0.70       | 90.5%          |
| Box Prompt        | 0.72  | 0.78       | 93.1%          |
| Automatic Prompt  | 0.59  | 0.66       | 88.7%          |

Box prompts performed best in guiding accurate segmentation in pancreatic CT/MRI scans.

---

##  Meeting Summaries

| Date | Summary |
|------|---------|
| **March 18, 2025** | Initial supervisor contact. Assigned tasks: research vision transformers and explore open-source medical imaging datasets. |
| **March 22, 2025** | First meeting. Decided on bi-weekly check-ins and focus on CT, PET, and MRI datasets using AI prompting. |
| **March 25, 2025** | Tasked to organize the GitHub repo and document datasets/models used. |
| **April 3, 2025**  | Positive feedback. Instructed to enrich documentation, include CT vs MRI comparisons, and begin SAM-based segmentation experiments. |

---

##  Author

**Olihi Idikwu**  
Final-year Software Engineering Student  
Macquarie University  
GitHub: [@manlikeolihi](https://github.com/manlikeolihi)

---

##  Citation

> Idikwu, O. (2025). *Deep Learning for Medical Imaging: Segmenting Pancreatic Cancer Using Prompt-Based Models*. Macquarie University.

---

##  Contact

For questions or collaboration, connect via [LinkedIn](https://www.linkedin.com/in/olihi-idikwu-007/).




