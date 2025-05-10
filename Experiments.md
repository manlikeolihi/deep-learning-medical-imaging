# Experiments

## 1. Data Preparation

The dataset used consists of CT and MRI images related to pancreatic cancer. Images were resized to 256×256 pixels and normalized. Ground truth masks were converted to binary form for comparison.

A 70/30 train-test split was applied to ensure balanced evaluation.

---

## 2. Mask Types

The Segment Anything Model (SAM) supports:
- **Point Prompts**: Single-click guidance
- **Box Prompts**: Object-enclosing bounding boxes
- **Automatic Masks**: Generated without manual input

Each prompt method was tested for effectiveness in medical segmentation.

---

## 3. Evaluation Metrics

We used:
- **Intersection over Union (IoU)**
- **Dice Score (DSC)**
- **Pixel Accuracy**

Formulas:

math
IoU = (Prediction ∩ GroundTruth) / (Prediction ∪ GroundTruth)
DSC = 2 × (Prediction ∩ GroundTruth) / (Prediction + GroundTruth)


##Baseline and Improvements

Baseline = SAM using point prompts.
Improvements tested:

Box prompts

Automatic masks

Post-processing with morphological closing

## Results

| Prompt Type      | IoU  | Dice Score | Pixel Accuracy |
| ---------------- | ---- | ---------- | -------------- |
| Point Prompt     | 0.64 | 0.70       | 90.5%          |
| Box Prompt       | 0.72 | 0.78       | 93.1%          |
| Automatic Prompt | 0.59 | 0.66       | 88.7%          |
