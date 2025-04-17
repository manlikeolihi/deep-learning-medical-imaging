
# Deep Learning for Medical Imaging – Pancreatic Cancer Focus




# data.md – Dataset Overview and Modalities

## 3.1 Comparison Between CT and MRI Data

### Visual Comparison

![CT vs MRI Modalities](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/CT_and_MRI_comparison.svg/1200px-CT_and_MRI_comparison.svg.png)

> **Source**: Wikimedia Commons ([Link](https://commons.wikimedia.org/wiki/File:CT_and_MRI_comparison.svg))

### Key Differences Between CT and MRI

| Aspect                 | CT (Computed Tomography)                                   | MRI (Magnetic Resonance Imaging)                            |
|------------------------|-------------------------------------------------------------|-------------------------------------------------------------|
| Modality Type          | X-ray based (ionizing radiation)                           | Magnetic fields and radio waves (non-ionizing)              |
| Image Clarity          | High resolution for bones, lungs, dense tissues            | High contrast for soft tissues (e.g., brain, pancreas)       |
| Scan Speed             | Faster (seconds to minutes)                                | Slower (minutes to tens of minutes)                         |
| Use Cases              | Trauma, lung/bone imaging, cancer screening                | Brain, muscle, spine, abdominal organ segmentation          |
| Radiation Exposure     | Yes                                                        | No                                                          |
| Cost and Availability  | Widely available, less expensive                          | More expensive, limited availability                        |

## 3.2 Dataset Summary Table

The following datasets were also referenced in the `models.md` file and were used in the evaluation or benchmarking of the deep learning segmentation models. These datasets are publicly available and highly relevant to pancreas or multi-organ segmentation tasks.

| Dataset Name                                                                 | Modality | Data Size      | # of Samples | Image Size        |
|------------------------------------------------------------------------------|----------|----------------|---------------|--------------------|
| [BTCV (Beyond the Cranial Vault)](https://www.synapse.org/#!Synapse:syn3193805) | CT       | ~10 GB         | 50            | 512×512×N slices   |
| [MSD Task07: Pancreas](http://medicaldecathlon.com/)                        | CT       | ~5 GB          | 420           | 512×512×N slices   |
| [NIH Pancreas Dataset](https://wiki.cancerimagingarchive.net/display/Public/Pancreas-CT) | CT       | ~12 GB         | 82            | Varies (512×512×N) |
| [BraTS 2021](https://www.med.upenn.edu/sbia/brats2021/data.html)           | MRI      | ~200 GB        | ~2000         | 240×240×155 voxels |
| [AMOS 2022](https://amos22.grand-challenge.org/)                            | CT + MRI | ~180 GB        | 500 (CT + MRI)| 512×512×N slices   |


