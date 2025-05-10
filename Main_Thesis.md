# Deep Learning for Medical Imaging: Segmenting Pancreatic Cancer Using Prompt-Based Models

## Abstract

This thesis investigates the application of prompt-based deep learning techniques to medical image segmentation, with a focus on pancreatic cancer. Using the Segment Anything Model (SAM) developed by Meta AI, the project evaluates different prompt types — point, box, and automatic — and measures segmentation performance using Intersection over Union (IoU), Dice Score, and Pixel Accuracy. The findings suggest that spatial prompts, such as bounding boxes, offer the most accurate segmentation results for this task.

---

## 1. Introduction

Pancreatic cancer remains one of the deadliest cancers, with early diagnosis heavily reliant on accurate medical imaging interpretation. Manual segmentation of medical scans is time-consuming and subject to variability. This project explores whether general-purpose, prompt-based segmentation models can be repurposed for medical imaging with minimal fine-tuning.

We aim to assess the effectiveness of prompt-guided segmentation for CT and MRI scans, particularly focusing on pancreatic cancer regions, using the Segment Anything Model (SAM).

---

## 2. Related Work

A full review of relevant literature from CVPR, ECCV, and MICCAI over the last five years is available in [literature_review.md](./literature_review.md). It includes studies on:

- Deep convolutional neural networks (CNNs) for medical segmentation
- Transformer-based approaches
- Foundation models applied to biomedical data
- Comparative analyses between CT and MRI imaging

---

## 3. Methodology

Details about the model (Segment Anything), its structure, and modifications are explained in [models.md](./models.md).

In brief:
- The project leverages SAM's zero-shot segmentation capability
- Prompts are used to guide the segmentation process
- Results are compared across different prompt types

---

## 4. Experimental Setup

For a detailed breakdown of experimental methods, see [experiments.md](./experiments.md).

- Data preparation and preprocessing
- Prompt types (point, box, auto)
- Evaluation metrics (IoU, Dice, Accuracy)
- Results comparison

The environment used for these experiments is detailed in [environment_setup.md](./environment_setup.md).

---

## 5. Results and Discussion

From the experiments, we observed:

| Prompt Type       | IoU   | Dice Score | Pixel Accuracy |
|-------------------|-------|------------|----------------|
| Point Prompt      | 0.64  | 0.70       | 90.5%          |
| Box Prompt        | 0.72  | 0.78       | 93.1%          |
| Automatic Prompt  | 0.59  | 0.66       | 88.7%          |

Box prompts produced the best results across all metrics, highlighting the importance of spatial guidance in segmenting medical images, even when using general-purpose models like SAM.

This confirms the hypothesis that lightweight prompt engineering can significantly enhance segmentation outcomes for complex medical tasks.

---

## 6. Conclusion

This thesis demonstrates that general-purpose segmentation models like SAM can be adapted for medical imaging applications through the strategic use of prompts. Among the prompt types tested, box prompts yielded the highest segmentation performance. Future work could explore fine-tuning SAM on labeled medical datasets and integrating clinical metadata for context-aware segmentation.

---



## References

1. Kirillov, A., et al. (2023). Segment Anything. Meta AI. https://segment-anything.com/
2. Ronneberger, O., Fischer, P., & Brox, T. (2015). U-Net: Convolutional Networks for Biomedical Image Segmentation. MICCAI.
3. Zhou, Z., Siddiquee, M.M.R., Tajbakhsh, N., & Liang, J. (2018). UNet++: A Nested U-Net Architecture for Medical Image Segmentation.
4. Isensee, F., et al. (2021). nnU-Net: Self-adapting Framework for U-Net-based Medical Image Segmentation.
5. Dosovitskiy, A., et al. (2020). An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale.

