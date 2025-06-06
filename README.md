

---

```markdown
# 🎭 Emotion Recognition Project

This project explores facial emotion recognition across five stages, from basic classification using FER+ to more advanced tasks such as personalized fine-tuning and attention-state emotion detection. The models are built using PyTorch and pretrained CNN architectures such as VGG19, ResNet50, and MobileNet.

---

## 📑 Project Structure

```

emotion\_project/
├── datasets/                # All datasets (FER+, RAF-DB, JAFFE, custom)
├── models/                  # Saved models (.pt/.h5) - NOT pushed to GitHub
├── notebooks/               # Jupyter notebooks for each project stage
├── results/                 # Visual outputs, confusion matrices, charts
├── .gitignore               # Ignore datasets/models/checkpoints
├── requirements.txt         # Python dependencies
└── README.md                # This file

````

---

## 🚀 Staged Development

### ✅ Stage 1: Basic Emotion Recognition
- **Dataset:** FER+
- **Model:** VGG19 (ImageNet-pretrained)
- **Goal:** Classify 7 basic emotions
- **Notebook:** `01_basic_model.ipynb`
- **Output:** Confusion matrix, prediction demo

### ✅ Stage 2: Multi-Dataset or Multi-Model Comparison
- **Options:**
  - A. Same model across datasets: FER+, RAF-DB, JAFFE
  - B. Same dataset across models: VGG19, ResNet50, MobileNet
- **Notebook:** `02_multi_model_dataset.ipynb`
- **Output:** Accuracy comparison bar chart, confusion matrices

### ✅ Stage 3: 3x3 Cross Combinations
- **Goal:** 3 datasets × 3 models = 9 total models
- **Notebook:** `03_cross_combinations.ipynb`
- **Output:** Summary table, 9 confusion matrices

### ✅ Stage 4: Personalized Model Fine-Tuning
- **Data:** 70 self-collected face images (7 emotions × 10 images)
- **Process:** Manual labeling → fine-tuning base model
- **Notebook:** `04_personal_finetune.ipynb`
- **Output:** Personal model performance, error case analysis

### ✅ Stage 5: Learning-State Emotion Classification
- **Objective:** Distinguish emotional states such as "focused", "distracted", etc.
- **Data:** Custom or public datasets (e.g., EmotiW, DEAP)
- **Notebook:** `05_attention_model.ipynb`
- **Output:** Demo predictions, confusion matrix

---

## 🧪 Sample Results

> All results are stored in `results/`, organized by stage:

- `results/confusion_matrix/stage*/` – confusion matrices  
- `results/demo_predictions/stage*/` – prediction samples  
- `results/charts/stage*/` – comparison visuals  

---

## 🔧 Dependencies

Install dependencies via:

```bash
pip install -r requirements.txt
````

Core libraries used:

* `torch`, `torchvision`
* `scikit-learn`
* `numpy`, `pandas`
* `opencv-python`
* `matplotlib`, `jupyter`

---

## 📂 Datasets

> Datasets are not included in this repository due to size and copyright.

Please manually download and place them under `datasets/`:

* [FER+](https://github.com/Microsoft/FERPlus)
* [RAF-DB](https://www.whdeng.cn/RAF/model1.html)
* [JAFFE](https://zenodo.org/record/3451524)
* Personal / Attention-state datasets: collected manually

Example structure:

```
datasets/
├── FER+/
├── RAF-DB/
├── JAFFE/
├── my_faces/
└── attention_dataset/
```

---

## 🧠 Highlights

* ✅ Modular notebook structure (stage-by-stage)
* ✅ Transfer learning with pretrained CNNs
* ✅ Support for personal data & label-driven fine-tuning
* ✅ Advanced state classification (beyond basic emotions)

---

## 📌 Notes

* Models are saved under `models/` but are **not committed** to GitHub (see `.gitignore`).
* For large datasets or models, please use Google Drive or Hugging Face Datasets to share.

---

## ✍️ Author

Ricky Chen – [GitHub Profile](https://github.com/rickychen0606)
National Chung Hsing University
2025 Spring – Artificial Intelligence Final Project


