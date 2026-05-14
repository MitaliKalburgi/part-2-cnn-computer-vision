# Computer Vision Problem Formulation and CNN Prototype

## Project Overview

This project formulates a computer vision problem from an image-based manufacturing defect dataset and builds a CNN prototype to classify product surface conditions into four categories: normal, scratch, dent, and stain.

---

## 📂 Dataset

The dataset used in this project is sourced from the shared Google Drive folder:

[Click here to access the dataset](https://drive.google.com/drive/folders/1akV6po4Nrgkc3yQrJkzA6cJlV-wBvUYs?usp=sharing)


---

## Repository Structure

- `notebook.ipynb` — main project notebook with all tasks
- `results/` — output files from model training
  - `accuracy_loss_curves.png` — training and validation accuracy/loss graphs
  - `confusion_matrix.png` — model evaluation confusion matrix
- `sample_predictions/` — visual output of model predictions
  - `prediction_outputs.png` — sample test images with predicted labels
- `requirements.txt` — required Python libraries
- `README.md` — project documentation

---

## Tasks Implemented

**Task 1 — Problem Identification**
Identified the problem as Image Classification — the model assigns one of four defect labels to each product image without needing to locate or outline the defect.

**Task 2 — Dataset Exploration**
Analysed class distribution, image dimensions, sample images from each class, and checked for class imbalance across the four categories.

**Task 3 — Image Preprocessing**
Images resized to 96x96 pixels, pixel values normalized to 0–1 range, and data split into 80% training and 20% testing sets using labels.csv.

**Task 4 — CNN Model Creation**
Built a Sequential CNN with two Conv2D layers, MaxPooling, Flatten, Dense, and a Softmax output layer for four-class classification.

**Task 5 — Model Training and Evaluation**
Trained for 20 epochs with Adam optimizer. Achieved 96.88% test accuracy. Outputs include accuracy/loss curves, confusion matrix, and sample predictions.

---

## 🛠 Technologies Used

- 🐍 Python
- 📓 Jupyter Notebook
- 🐼 Pandas — data manipulation
- 🔢 NumPy — numerical computations
- 📊 Matplotlib — plotting and visualisation
- 🎨 Seaborn — confusion matrix visualisation
- 🤖 Scikit-learn — train/test split and evaluation metrics
- 🧠 TensorFlow / Keras — CNN model building and training
- 🖼 Pillow — image loading and preprocessing

---

## ▶️ How to Run

1. Download the dataset from the link above and place the `images/` folder and 
`labels.csv` in the project directory
2. Open `notebook.ipynb` in Jupyter Notebook or VS Code
3. Run all cells in order
4. Outputs will be saved to the `results/` and `sample_predictions/` folders

---

## 📝 Notes

- Dataset files and model outputs are not included in this repository
- The model achieves 91.67% test accuracy across four defect classes
