📁 Project Structure
datasets/ – All datasets used in this project

FER+/ – Public dataset for basic emotion classification

RAF-DB/, JAFFE/ – Additional datasets for multi-source training

my_faces/ – Your own labeled facial images (used in Stage 4)

attention_dataset/ – Custom learning-state emotion data (Stage 5)

models/ – Saved model checkpoints (.pt, .h5)
(ignored via .gitignore, stored locally or in cloud)

ferplus_vgg19.pt, rafdb_resnet.pt, personal_model.pt, etc.

notebooks/ – Jupyter notebooks for each stage

01_basic_model.ipynb – Stage 1: FER+ + VGG19

02_multi_model_dataset.ipynb – Stage 2: Multi-model or multi-dataset

03_cross_combinations.ipynb – Stage 3: 3×3 model/dataset combos

04_personal_finetune.ipynb – Stage 4: Fine-tune on personal data

05_attention_model.ipynb – Stage 5: Learning-state classification

results/ – Output images, confusion matrices, comparison charts

confusion_matrix/stage1~5/ – Each model’s confusion matrix

demo_predictions/stage1, 4, 5/ – Visual prediction results

charts/stage2~3/ – Accuracy, F1-score charts

.gitignore – Ignore rules for datasets, models, and cache

requirements.txt – Required Python packages

README.md – Project documentation (you’re reading it now)