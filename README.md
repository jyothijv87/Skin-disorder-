# Skin-disorder-
Classifying  type of skin disorder by using different  supervised classification models  and comparing the results among the models

## Project Overview
This project aims to build a **machine learning model** to classify various skin disorders using **tabular clinical or numerical data**. The goal is to provide accurate preliminary diagnosis support based on patient attributes, symptoms, or lab results.

---

## Dataset
- Contains numerical features such as age, symptom scores, skin measurements, lab results, etc.
- **Target variable:** Skin disorder class (e.g., eczema, psoriasis, acne, fungal infection, etc.)
- **Number of features:34
- **Number of samples:366
- **Dataset source:** Datamites

---

## Features
- Data preprocessing: missing value handling, scaling, encoding categorical variables
- Feature selection (optional)
- Classification using models like:
  - Random Forest
  - XGBoost
   - Logistic Regression
- Model evaluation metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix

---

## Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/skin-disorder-tabular.git
```
2. Navigate to the project directory:
```bash
cd skin-disorder-tabular
```
3. Install dependencies:
```bash
pip install -r requirements.txt
```

---

## Usage
- **Train the model:**
```bash
python train.py --data_path path_to_dataset.csv
```
- **Evaluate the model:**
```bash
python evaluate.py --model_path path_to_saved_model.pkl
```
- **Predict new sample(s):**
```bash
python predict.py --input data/sample_input.csv --model path_to_saved_model.pkl
```

---

## Modeling Approach
- Models trained on **numerical/tabular features**
- Feature scaling using **StandardScaler** or **MinMaxScaler**
- Training-validation split: 80-20
- Metrics tracked during evaluation: Accuracy, Precision, Recall, F1-score
- Optional: Hyperparameter tuning using GridSearchCV or RandomizedSearchCV

---

## Results
- **Best Model:** Random Forest (or your chosen model)
- **Training Accuracy:** 98%
- **Validation Accuracy:** XX%
- Confusion matrix stored in `/results` folder

---

## Folder Structure
```
skin-disorder-tabular/
│
├── data/                  # CSV dataset files
├── models/                # Saved trained models
├── scripts/               # Training, evaluation, prediction scripts
├── results/               # Metrics, confusion matrices
├── notebooks/             # Jupyter notebooks (optional)
├── requirements.txt       # Dependencies
└── README.md              # Project overview
```

---

## Contributing
- Fork the repository, make improvements, and submit pull requests
- Report issues via GitHub Issues for bugs or suggestions

---

## License
This project is licensed under the **MIT License**
