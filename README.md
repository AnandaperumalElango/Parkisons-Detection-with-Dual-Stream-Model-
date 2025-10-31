

---

```markdown
# 🧠 Enhancing Parkinson’s Disease Detection with a GAN-CNN Hybrid Dual Stream Model

**Author:** E. Anandaperumal  
**Published in:** *EAI Endorsed Transactions on Pervasive Health and Technology*  
**DOI:** [10.4108/eai.28-4-2025.2357835](https://eudl.eu/doi/10.4108/eai.28-4-2025.2357835)

---

# 📘 Overview

This repository contains the implementation of the research work **“Enhancing Parkinson’s Disease Detection with a GAN-CNN Hybrid Dual Stream Model.”**  
The proposed model combines **Generative Adversarial Networks (GANs)** and **Convolutional Neural Networks (CNNs)** to improve the diagnostic accuracy of Parkinson’s Disease (PD) from MRI images.

The model employs a **dual-stream architecture** — one stream trained on real MRI data and the other on GAN-generated synthetic data.  
By fusing the learned features from both streams, the system enhances generalization and robustness in medical image classification.

---

# 🧩 Key Features

- 🧬 Dual-stream design combining real and synthetic MRI data.  
- ⚙️ GAN for data augmentation to overcome class imbalance.  
- 🔍 CNN classifier for accurate Parkinson’s disease detection.  
- 📈 Improved accuracy and F1-score compared to baseline CNNs.  
- 📊 Grad-CAM visualization for interpretability.

---

# 🧠 Model Architecture



```
     +-------------------+
     |   MRI Dataset     |
     +---------+---------+
               |
               v
      +----------------+
      |     GAN Model   |
      +--------+--------+
               |
    +----------+----------+
    |                     |
Real Image Stream     Synthetic Image Stream
|                     |
+----------+----------+
|
Feature Fusion Layer
|
Classification

```



# 🧪 Methodology

1. **Data Preprocessing:** Normalize and resize MRI images.  
2. **GAN Training:** Generate high-quality synthetic MRI data.  
3. **CNN Training:** Dual CNNs trained on real and synthetic streams.  
4. **Feature Fusion:** Combine learned features for classification.  
5. **Evaluation:** Accuracy, Precision, Recall, F1-score, ROC-AUC.

---

# 🧰 Technologies Used

| Component | Framework / Library |
|------------|--------------------|
| Language | Python |
| Deep Learning | Pytorch |
| Data Handling | NumPy, Pandas |
| Visualization | Matplotlib, Seaborn |
| Image Processing | OpenCV |
| Model Evaluation | Scikit-learn |

---

# 📂 Repository Structure

```

📁 Parkinsons_Detection_GAN_CNN/
│
├── 🧠 parkisons_detection_with_GAN&CNN.ipynb   # Main implementation
├── 📜 Enhancing Parkinsons Disease Detection with a GAN-CNN hybrid Dual Stream Model.pdf
├── 📊 results/                                 # Model outputs and metrics
└── 📄 README.md                                # Documentation

````

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/Parkinsons_Detection_GAN_CNN.git
   cd Parkinsons_Detection_GAN_CNN
````

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebook**

   ```bash
   jupyter notebook parkisons_detection_with_GAN&CNN.ipynb
   ```

---

## 📈 Results

| Metric    | GAN-CNN Dual Stream | Baseline CNN |
| --------- | ------------------- | ------------ |
| Accuracy  | **97.8%**           | 92.3%        |
| Precision | 96.5%               | 90.7%        |
| Recall    | 98.1%               | 91.2%        |
| F1-Score  | 97.3%               | 91.0%        |

> The dual-stream GAN-CNN model achieved a 5–6% higher accuracy than traditional CNNs.

---

## 🧩 Citation

If you use this repository, please cite:

```
@article{eai2025ganparkinsons,
  title={Enhancing Parkinson’s Disease Detection with a GAN-CNN Hybrid Dual Stream Model},
  author={E. Anandaperumal},
  journal={EAI Endorsed Transactions on Pervasive Health and Technology},
  year={2025},
  doi={10.4108/eai.28-4-2025.2357835}
}
```

---

## 💡 Future Work

* Integrate attention-based CNNs for improved localization.
* Expand dataset to include multimodal imaging.
* Deploy as a real-time diagnostic web app.

---

## 🧑‍⚕️ Acknowledgments

This research by **E. Anandaperumal** contributes to advancing AI-based medical diagnosis.
The hybrid GAN-CNN dual-stream approach offers a significant step toward reliable and explainable Parkinson’s disease detection.

---


