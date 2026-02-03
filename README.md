et---

# 🧠 Breast Cancer Classification using IQI-BGWO-SVM

*A Machine Learning and Metaheuristic Optimization Approach on the MIAS Dataset*

---

## 📌 Project Overview

This repository presents a full pipeline for **automated breast cancer classification** using a hybrid approach that combines:

* 🧮 **Support Vector Machines (SVM)** for classification
* 🐺 **Improved Quantum-Inspired Binary Grey Wolf Optimizer (IQI-BGWO)** for optimal feature selection and hyperparameter tuning

The model is applied to the **Mammographic Image Analysis Society (MIAS)** dataset, which contains annotated mammograms labeled as benign or malignant. Our work reproduces and extends results from recent literature, focusing on diagnostic accuracy, model interpretability, and optimization efficiency.

---

## 📂 Repository Structure

```
📁 IQI-BGWO-SVM-MIAS
├── 📜 README.md               ← Project overview
├── 📊 results/                ← Output images: charts, plots, ROC curves
├── 📁 code/
│   ├── IQI_BGWO_SVM.ipynb     ← Main notebook: preprocessing, feature extraction, modeling
│   ├── utils.py               ← ROI extraction, data loaders, preprocessing
│   └── optimization.py        ← IQI-BGWO implementation
├── 📁 data/
│   ├── MIAS/                  ← Raw and preprocessed MIAS images
│   └── truth_data.csv         ← Parsed MIAS annotations
└── 📄 final_report.docx       ← Full academic paper (APA-style)
```

---

## 🧪 Features & Methods

* 📸 ROI extraction using MIAS ground-truth lesion coordinates
* 📈 Texture, shape, and intensity feature extraction (GLCM, LBP, entropy, etc.)
* 🔍 SVM classifier with RBF kernel
* ⚙️ IQI-BGWO metaheuristic optimization

  * Binary feature selection
  * Hyperparameter tuning (`C`, `σ`)
* 📊 Evaluation: Accuracy, Sensitivity, Specificity, ROC-AUC
* 🧠 Visualizations: Feature importance, ROC curves, performance charts

---

## 📊 Results

| Model               | Accuracy  | Sensitivity | Specificity | ROC-AUC   |
| ------------------- | --------- | ----------- | ----------- | --------- |
| Logistic Regression | 83.2%     | 82.5%       | 83.7%       | 0.865     |
| SVM (RBF)           | 88.1%     | 87.2%       | 88.9%       | 0.903     |
| **IQI-BGWO-SVM**    | **92.5%** | **91.3%**   | **93.4%**   | **0.942** |

---

## 🛠️ How to Run

1. **Clone the repo**

```bash
git clone https://github.com/your-username/IQI-BGWO-SVM-MIAS.git
cd IQI-BGWO-SVM-MIAS
```

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Open the main notebook**

```bash
jupyter notebook code/IQI_BGWO_SVM.ipynb
```

4. **Run cells in order**
   This will:

* Preprocess data
* Extract features
* Run SVM or IQI-BGWO-SVM
* Evaluate and visualize results

---

## 📄 Documentation

* `final_report.docx`: A full research paper with all methods, results, and analysis
* Annotated code and comments inside the notebook
* Visualization outputs stored in `/results/` folder

---

## 📚 References

* Bilal, A. et al. (2024). *Breast cancer diagnosis using support vector machine optimized by improved quantum inspired grey wolf optimization*. Scientific Reports, 14, 10714.
* MIAS Dataset: [http://peipa.essex.ac.uk/info/mias.html](http://peipa.essex.ac.uk/info/mias.html)

---

## 📬 Contact & Contributions

Feel free to fork the repository or raise issues. Contributions and improvements are welcome!

📧 Email: [musa39078@gmail.com](mailto:musa39078@gmail.com)
👨‍💻 Maintainer:Ghulam Mustafa

---
