# Comparative Analysis of NiN and Multi‑Branch Networks

This project presents a comparative study of **Network‑in‑Network (NiN)** and a **multi‑branch GoogLeNet‑style architecture** for multiclass image classification and transfer learning. It was developed as a case study using the **Sign‑MNIST** dataset and extended to **MNIST** for transfer learning.

---

## 📊 Project Description

The goal is to evaluate two different deep neural architectures in terms of accuracy, convergence, parameter efficiency, and transferability.

### Datasets

* **Sign‑MNIST**
* **MNIST**

### Architectures

* **Network‑in‑Network (NiN)** – Uses 1×1 convolutions (mini‑MLPs) within convolutional layers to enhance nonlinear feature learning.
* **Multi‑Branch Network (GoogLeNet‑style)** – Employs parallel convolutional branches (1×1, 3×3, 5×5, pooling) to capture multi‑scale features.

### Tasks

1. Train and evaluate NiN and GoogLeNet on **Sign‑MNIST**.
2. Apply **transfer learning** by adapting both models to **MNIST**.
3. Compare performance using accuracy, precision, recall, F1‑score, and resource requirements.

---

## 🛠 Requirements

Install the dependencies to run the project:

```bash
pip install -r requirements.txt
```

---

## 📈 Results

* On **Sign‑MNIST**:

  * NiN achieved ≈ **98.37% accuracy** with \~180k parameters.
  * GoogLeNet achieved ≈ **93.61% accuracy** with \~37k parameters.
* On **MNIST (Transfer Learning)**:

  * NiN achieved ≈ **82.88% accuracy**.
  * GoogLeNet achieved ≈ **92.64% accuracy**.

**Key Insight:** NiN excels on the original dataset with higher accuracy, but GoogLeNet generalizes better in transfer learning with fewer parameters.

