# Orthogonal Gradient Guided Test-Time Training (OGG-TTT)

This repository will host the official code for the paper:

**Orthogonal Gradient Guided Test-Time Training for Source-Free Domain Adaptation in Echocardiographic Video Segmentation**

> **📌 Note:** This repository is currently under preparation and will be released upon publication of the paper.

---

## 🧠 Overview

Deploying deep neural networks in real-world medical scenarios often faces **performance degradation** due to **domain shift**—especially when **source domain data is inaccessible** due to privacy regulations. 

To address this, **Test-Time Training (TTT)** allows real-time model adaptation using **unlabeled target data during inference**. While effective in natural image segmentation, conventional TTT approaches based on **Self-Supervised Learning (SSL)** and **Pseudo-Label Supervised Learning (PSL)** face limitations when applied to **Source-Free Domain Adaptation (SFDA)** in echocardiographic video segmentation.

---

## 🚀 Contributions

This work introduces:

- **Gradient Orthogonality Constraint (GOC):**  
  Dynamically adjusts the influence of SSL based on the alignment of SSL and PSL gradients, avoiding interference and overfitting.
  
- **Decoupled Pseudo-Label Supervision:**  
  Separates the learning of domain-invariant and domain-specific features to stabilize adaptation.

- **Robust TTT Framework for Medical Videos:**  
  Designed and validated on **three echocardiographic video datasets** from different hospitals, with varying imaging devices and patient demographics.

---

## 📊 Highlights

- Significantly outperforms previous state-of-the-art methods in **source-free domain adaptation echocardiographic video segmentation**.
- Improves **stability**, **accuracy**, and **adaptability** of test-time domain adaptation under real clinical domain shifts.

---

## 🧪 Datasets

Experiments are conducted on three public echocardiographic datasets. Details and preprocessing instructions will be included upon code release.

---

## 📁 Project Structure (To be updated)

```bash
OGG-TTT/
├── models/              
├── losses/             
├── datasets/            
├── utils/               
├── configs/             
├── test_time_train.py   
├── train_source.py      
├── evaluate.py          
├── requirements.txt     
└── README.md            
