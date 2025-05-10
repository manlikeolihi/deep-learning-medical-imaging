
# Thesis: Deep Learning for Medical Imaging – Segmentation of Pancreatic Cancer

## Abstract

This thesis explores the use of deep learning methods for semantic segmentation of medical images, with a specific focus on pancreatic cancer. By leveraging Meta AI's Segment Anything Model (SAM), we evaluate how prompt-based segmentation can be applied to CT and MRI data. We compare various prompt types, analyze performance metrics, and explore improvements for medical image segmentation.

---

## 1. Introduction

Medical imaging plays a crucial role in cancer diagnosis, but manual segmentation is time-consuming and error-prone. This thesis investigates the use of prompt-based deep learning methods — specifically SAM — to automate and improve segmentation in pancreatic cancer scans.


## 2. Related Work

See [literature_review.md](./literature_review.md) for a summary of recent research from CVPR, ECCV, MICCAI, and other top venues, focusing on semantic segmentation models and medical applications.


## 3. Methodology

Details of the Segment Anything Model architecture and custom modifications are documented in [models.md](./models.md).


## 4. Experiments

Experimental setup, mask evaluation, and metric results are documented in [experiments.md](./experiments.md).  
The environment configuration is available in [environment_setup.md](./environment_setup.md).



## 5. Results and Discussion

The best-performing method was the box prompt, achieving the highest Dice Score and Pixel Accuracy. This confirms the usefulness of spatial priors in guiding segmentation in medical contexts.

Further exploration could involve fine-tuning SAM on medical datasets or integrating clinical metadata to enhance performance.


## 6. Conclusion

This study demonstrates that foundation models like SAM can be adapted to medical imaging with minimal modification. Prompt-based segmentation offers a scalable, efficient alternative to manual annotation, particularly in resource-limited healthcare environments.



## References

1. Kirillov, A., et al. (2023). Segment Anything. Meta AI.
2. [Add 4–6 key papers from your `literature_review.md` here]
