# Smart Home Data Anonymization using Convolutional Autoencoders

This project explores the use of **deep learning techniques to anonymize smart home sensor data** while preserving useful patterns for analysis.

Smart home environments collect large volumes of sensitive time-series data from sensors and devices. Protecting user privacy while maintaining the usefulness of this data is an important challenge.

This project applies a **1D Convolutional Autoencoder (CAE)** implemented in **PyTorch** to learn a compressed representation of smart home sensor data.

---

## Objective

The objectives of this project are:

- analyze smart home sensor time-series data
- build sliding windows from the dataset
- train a convolutional autoencoder model
- reconstruct anonymized versions of the data
- evaluate reconstruction error
- visualize differences between original and reconstructed data

---

## Dataset

The dataset contains **smart home sensor readings with weather information**.

Typical attributes include:

- sensor measurements
- device states
- environmental variables
- time-series observations

Due to file size limitations, the dataset is **not included in this repository**.

Place the dataset file in the project folder:
