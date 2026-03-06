
# Privacy-Preserving Data Science Projects

Author: Marios Vardalachakis

This repository holds a variety of data science and machine learning notebooks, particularly focused on privacy-preserving techniques, as well as anomaly detection.

The notebooks in this repository introduce various techniques used to ensure the privacy of sensitive information while still being informative enough to perform analysis on it.

The topics covered in this repository are:

- classical data anonymization
- privacy-preserving fraud detection
- deep learning-based smart home data anonymization


---

# Projects

## Classical Data Anonymization


This project aims to introduce traditional anonymization techniques used to ensure the privacy of sensitive information within a structured dataset.

The techniques used in this project include:

-k-Anonymity
-l-Diversity
-t-Closeness

The project compares different anonymization strategies and evaluates their effect on data utility and retention.

### Example Result

<p align="center">
  <img src="projects/classical-anonymization/Anonymization_comparison.png" width="600"/>
</p>


Project folder:

```
projects/classical-anonymization
```

---

## Privacy-Preserving Fraud Detection

This project investigates fraud detection while applying modern privacy-preserving machine learning techniques.

Three privacy scenarios are explored:

- Generative Adversarial Networks (GANs) for synthetic data generation
- Differential Privacy using Opacus
- Federated Learning simulation

These methods allow models to be trained while reducing exposure of sensitive financial data.

Project folder:

```
projects/privacy-scenarios-fraud-detection
```

---
### Example Result

Visualization comparing real data with GAN-generated synthetic samples using PCA.

<p align="center">
  <img src="projects/fraud-detection/real_vs_synthetic.png" width="600"/>
</p>


## Smart Home Data Anonymization using Autoencoders

This project applies deep learning techniques to smart home sensor data.

A 1D Convolutional Autoencoder implemented in PyTorch is used to learn compressed representations of time-series sensor data.

The model attempts to preserve useful information while reducing exposure of raw smart home activity patterns.

### Example Result

<p align="center">
  <img src="projects/smart-home-cae/reconstruction_error.png" width="600"/>
</p>

Project folder:

```
projects/smart-home-cae
```

---

# Repository Structure

```
kaggle-notebooks
│
├── README.md
├── requirements.txt
├── environment.yml
├── .gitignore
│
├── docs
│   ├── methodology.md
│   └── project_overview.md
│
└── projects
    ├── classical-anonymization
    ├── privacy-scenarios-fraud-detection
    └── smart-home-cae
```

Each project folder contains:

- a Jupyter notebook
- a project-specific README
- visualizations of results
- configuration files where needed

---

# Technologies Used

The projects in this repository use the following tools:

- Python
- Pandas
- NumPy
- Scikit-learn
- PyTorch
- Matplotlib
- Jupyter Notebook
- Differential Privacy (Opacus)

---

# Installation

Clone the repository:

```
git clone https://github.com/mariosvard/kaggle-notebooks.git
cd kaggle-notebooks
```

Install dependencies:

```
pip install -r requirements.txt
```

Run Jupyter Notebook:

```
jupyter notebook
```

---

# Data

Datasets are not included in this repository due to file size limitations.

Please download the datasets from their original sources and place them in the corresponding project folders before running the notebooks.

---

# Notes

This repository is intended as a data science portfolio demonstrating privacy-preserving machine learning techniques applied to different datasets.















