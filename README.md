# 🌊 AI SpillGuard: Oil Spill Detection

An AI-powered system to detect and monitor **oil spills** in satellite imagery using deep learning.
Developed as part of an **internship project**, this repository contains the dataset setup, preprocessing pipeline, visualization, and a baseline CNN model for oil spill classification.

---

## 📌 Project Overview

Oil spills pose severe risks to marine ecosystems and coastal economies. Traditional detection methods are slow and resource-intensive.
This project leverages **Convolutional Neural Networks (CNNs)** and later **U-Net segmentation models** to automatically identify and highlight oil-contaminated regions in satellite images.

---

## 📂 Dataset

* **Classes**:

  * `oilspill`
  * `nospill`
* **Structure**:

```
dataset/
│── train/
│   ├── nospill/   (81 samples)
│   └── oilspill/  (77 samples)
│
└── validation/
    ├── nospill/   (17 samples)
    └── oilspill/  (22 samples)
```

---

## 🛠️ Workflow

1. **Data Collection** → Kaggle dataset organized into train/validation splits
2. **Preprocessing** → Image resizing, normalization
3. **Augmentation** → Random flips, rotations, zooms for better generalization
4. **Visualization** → Side-by-side comparison of original vs augmented samples
5. **Model** → Baseline CNN classifier implemented
6. **Training** → Ongoing experiments on classification accuracy
7. **Next** → Segmentation with U-Net + Streamlit web app deployment

---

## 📊 Internship Milestones

* **Week 1–2** → Dataset setup, preprocessing & augmentation
* **Week 3–4** → Model development (CNN/U-Net), training pipeline
* **Week 5–6** → Evaluation (Accuracy, IoU, Dice, Precision, Recall)
* **Week 7–8** → Deployment via Streamlit, final documentation & presentation

---

## ⚙️ Requirements

* Python 3.9+
* TensorFlow 2.15+
* NumPy
* Matplotlib
* Jupyter
* Streamlit (for deployment stage)

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

1. **Clone repository**

   ```bash
   git clone https://github.com/yourusername/oil-spill-detection.git
   cd oil-spill-detection
   ```

2. **Open notebook**

   ```bash
   jupyter notebook cnn_pipeline.ipynb
   ```

3. **Run pipeline**

   * Preprocessing & augmentation
   * Visualization of original vs augmented samples
   * Train baseline CNN

4. **(Upcoming)** Run web app

   ```bash
   streamlit run app.py
   ```

---

## 👨‍💻 Author

Developed as part of internship by **Mohammad Afnan Mirza**


