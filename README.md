# AI-Powered Multitarget Drug Discovery using Deep Learning

## 🔬 Project Overview
This project aims to classify drug molecules based on their bioactivity against four protein targets using a deep learning model. Molecules are represented as SMILES strings and converted into Morgan fingerprints using RDKit's `MorganGenerator`. A dense neural network is trained to predict the target class of each compound.

---

## 📁 Files Included

| File Name                          | Description |
|-----------------------------------|-------------|
| `project_report.docx/pdf`         | Final project summary document |
| `drug_discovery_notebook.ipynb`   | Jupyter notebook with full pipeline |
| `protein_classifier_model.h5`     | Trained deep learning model |
| `molecule_classification_dataset.csv` | Source dataset from Kaggle |


---

## 📊 Dataset Used

- **Name**: [MultiTarget Bioactivity ChEMBL](https://www.kaggle.com/datasets/xjoannax88/multitarget-bioactivity-chembl)
- **Molecules**: ~8,700 compounds
- **Targets**: EGFR, HDAC2, PPARG, SRD5A2
- **Features**: SMILES, Molecular Weight, LogP, HBA, HBD, TPSA

---

## 🧠 Model Overview

- **Input**: 2048-bit Morgan fingerprints
- **Architecture**: Dense Neural Network (512 → 256 → 128 → Softmax)
- **Training**: 20 epochs, categorical crossentropy loss, Adam optimizer
- **Evaluation**: Accuracy, Confusion Matrix, Classification Report, t-SNE visualization

---

## 💡 Novelty in This Project

- Multitarget classification (not just binary)
- Use of modern `MorganGenerator` from RDKit
- Integrated exploratory data analysis (EDA)
- t-SNE for fingerprint visualization
- Clean, deployable pipeline

---

## 🎥 Code Explanation Video

📺 Watch here: [Insert Drive or YouTube Link]

---

## 📂 How to Run

1. Clone the repository or download the files
2. Open `drug_discovery_notebook.ipynb` in Jupyter
3. Install requirements:
   ```bash
   pip install rdkit pandas seaborn matplotlib scikit-learn tensorflow
