# 🌱 Soil Image Classification Challenge 2025

This repository contains the code and data processing pipeline for the **Soil Image Classification Challenge 2025** hosted by Annam.ai at IIT Ropar. The goal is to classify soil images into one of the following four categories:

- **Alluvial**
- **Black**
- **Clay**
- **Red**

---

## 📁 Project Structure
```bash
soil_classification-2025/
├── train/
├── test/ 
├── train_labels.csv 
├── test_ids.csv
├── Soil_Classification.ipynb 
└── submission.csv # Final model predictions for submission

```
## 🚀 Quick Start (on Google Colab)

### 🔗 Step 1: Mount Google Drive

Make sure the folder `soil_classification-2025` is placed inside your Google Drive.

```bash
/MyDrive/soil_classification-2025/
├── train/
├── test/
├── train_labels.csv
└── test_ids.csv
```
In the notebook, run the Google Drive mount cell:
from google.colab import drive
drive.mount('/content/drive')

### Step 2: Run All Cells in Soil_Classification.ipynb
````markdown
This notebook is structured to:

Load and preprocess the data

Create PyTorch datasets and loaders

Train a deep learning model using EfficientNet

Evaluate performance

Generate submission CSV

⏱️ Expected Training Time: ~30 minutes (5 epochs on Google Colab GPU)
````
## Model Architecture
````markdown
Backbone: EfficientNet-B0 (torchvision)

Image Size: 224x224

Optimizer: Adam (lr=1e-4)

Loss: CrossEntropyLoss (can switch to Focal Loss for imbalanced data)

Mixed Precision: torch.cuda.amp used for faster training
````
## 🧪 Evaluation
Metric	Score
F1-Score	0.9655
Target	1.0000

## ✍️ Author
Developed by a Aniket Raj of the Soil Image Classification Challenge 2025.

## 📜 License
For academic and research use only. All rights reserved to the original competition organizers and dataset providers.
### ✅ You can now:
- Paste this into `README.md` in your GitHub repo.
- Add badges or screenshots if you'd like polish (just let me know).

Need the actual `.md` file to upload directly or want me to include a preview image?
