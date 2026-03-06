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

before running the notebook.

---

## Method

### 1D Convolutional Autoencoder (CAE)

The model learns a compressed representation of time-series sensor data.

The architecture consists of two parts:

**Encoder**

- 1D convolution layers
- compresses the input sequence into a latent representation

**Decoder**

- reconstructs the original signal from the compressed representation

This transformation allows the model to **retain important patterns while reducing exposure of raw sensor data**.

---

## Workflow

The notebook performs the following steps:

1. Load the smart home dataset
2. Select numeric features
3. Normalize the data
4. Create sliding windows from the time-series
5. Train a 1D convolutional autoencoder
6. Reconstruct the input sequences
7. Measure reconstruction error
8. Visualize results

---

## Results

### Reconstruction Error

The following visualization shows the distribution of reconstruction errors between the original and reconstructed sequences.

![Reconstruction Error](figures/reconstruction_error.png)

### Interpretation

Low reconstruction error indicates that the model successfully learns the structure of the time-series data.

The compressed representation can help preserve useful patterns while reducing the exposure of sensitive raw data.

---

## Notebook

The full implementation is provided in:

The notebook includes:

- data preprocessing
- sliding window generation
- model architecture
- model training
- reconstruction analysis

---

## Technologies Used

The project was implemented using:

- Python
- PyTorch
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## Notes

This project demonstrates how **deep learning models such as convolutional autoencoders can be used for privacy-preserving analysis of smart home time-series data**.****


