# Privacy-Preserving Fraud Detection

This project explores fraud detection techniques while incorporating **privacy-preserving machine learning methods**.

The goal is to demonstrate how modern privacy techniques such as **Generative Adversarial Networks (GANs)**, **Differential Privacy**, and **Federated Learning** can be used when working with sensitive financial datasets.

---

## Objective

The objectives of this project are:

- analyze fraudulent transaction data
- generate synthetic data using GANs
- train models using differential privacy
- simulate federated learning training rounds
- evaluate the impact of privacy mechanisms on model performance

---

## Dataset

The dataset contains anonymized financial transaction records used for fraud detection.

Typical attributes include:

- transaction features
- anonymized numerical variables
- fraud labels (fraud / non-fraud)

Due to file size limitations, the dataset is **not included in this repository**.

You can download it from:

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Place the dataset in the project folder before running the notebook.

---

## Methods Explored

The notebook explores several modern machine learning and privacy techniques:

### Generative Adversarial Networks (GAN)

GANs are used to generate **synthetic financial data** that preserves statistical properties of the original dataset.

This helps address:

- class imbalance
- privacy concerns
- data scarcity

---

### Differential Privacy

The model is trained using **Differential Privacy (Opacus)** to protect sensitive information during training.

Differential privacy introduces noise into the training process to ensure that individual records cannot be reconstructed.

---

### Federated Learning Simulation

The notebook simulates **federated learning rounds**, where multiple nodes collaboratively train a model without sharing raw data.

This approach is useful in environments where data cannot be centrally stored.

---

## Visualizations

### GAN Synthetic Data vs Real Data (PCA Projection)

Visualization of real data and GAN-generated synthetic samples.

![GAN PCA Projection](real_vs_synthetic.png)

---

### Differential Privacy Training Performance

Comparison of model accuracy with and without differential privacy.

![Differential Privacy Accuracy](figures/dp_accuracy.png)

---

### Federated Learning Training Progress

Training accuracy across multiple federated learning rounds.

![Federated Learning Rounds](figures/fl_rounds.png)

---

## Notebook

The full implementation is provided in:

`Fraud_Detection_from_kagglee2.ipynb`

The notebook includes:

- data preprocessing
- GAN-based synthetic data generation
- differential privacy training
- federated learning simulation
- visualization of model performance

---

## Technologies Used

The project was implemented using:

- Python
- Pandas
- NumPy
- PyTorch
- Opacus (Differential Privacy)
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Notes

This project demonstrates how **privacy-preserving machine learning techniques** can be applied in fraud detection scenarios where sensitive financial data must remain protected.

