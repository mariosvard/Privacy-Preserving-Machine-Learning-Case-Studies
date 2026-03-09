# Privacy-Preserving Fraud Detection

This project aims to examine techniques in fraud detection, as well as techniques in privacy-preserving machine learning. The main purpose of this project is to show how these latest technologies in privacy can be used in analyzing financial transaction data.Technologies to be used in this project:

*   Generative Adversarial Networks (GANs)
*   Differential Privacy
*   Federated Learning

These technologies allow machine learning models to be trained without compromising financial data.


## Objective

The main objectives of this project are:

- To analyze financial transaction data, usually used in fraud detection
- To generate synthetic financial transaction data using GANs
- To train machine learning models using Differential Privacy
- To simulate Federated Learning rounds
- To examine how these techniques in privacy affect model performance


## Dataset

The experiments use the Credit Card Fraud Detection dataset, which can be found on the Kaggle platform.

**[Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)**


This dataset contains anonymized credit card transactions from European cardholders.

**Dataset Characteristics**

- transaction features
- anonymized numerical variables
- fraud labels (fraud / non-fraud)

**Typical Attributes**

The dataset includes:

- anonymized numerical transaction features (V1–V28)
- time of transaction
- amount of transaction
- label for fraudulent transactions (0 for legitimate, 1 for fraud)

  
Due to file size limitations, the dataset is **not included in this repository**.

You can download it from:

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

After downloading, place the data within the project directory before running the notebook.


## Methods Explored

The notebook employs a variety of state-of-the-art privacy-preserving machine learning techniques.

**Generative Adversarial Networks (GANs)**

Generative Adversarial Networks are employed for generating synthetic financial transactional data.

A GAN is composed of two competing artificial intelligence models:

- **Generator**: Used for generating synthetic data

- **Discriminator**: Used for distinguishing between real and synthetic data

As a result of the competition between the two models, the generator is trained to produce synthetic data that resembles the statistical properties of the original dataset.


**Benefits**

- Class imbalance in fraud detection datasets is overcome
- Data sharing is facilitated without the need for disclosing real financial information
- Privacy-preserving analysis of the data is facilitated

---

### Differential Privacy

The model is trained with the help of Differential Privacy with the help of the Opacus library.

Differential Privacy introduces noise into the entire training process so that no single transaction is identifiable.


**Key Properties**

- Individual transaction records are protected
- Information leakage from the models is limited
- Quantifiable privacy is ensured

The performance of the models with and without Differential Privacy is compared in this project to assess the privacy-utility tradeoff.



### Federated Learning Simulation

The notebook also includes the simulation of the Federated Learning rounds.

In federated learning:

- nodes are trained individually
- raw data is not transmitted
- only updates are transmitted

**Workflow**

- The dataset is split into multiple clients
- Each client is trained individually
- updates are aggregated
-  The global model is updated

This is similar to how financial systems are designed in the real world. Data is not sharable among institutions.


## Visualizations

The project includes various visualizations to assess the effectiveness of the proposed privacy-preserving approaches.

**GAN Synthetic Data vs Real Data**

Comparison between real transaction data and GAN-based synthetic data using PCA projection.

<div align="center"> <img src="real_vs_synthetic.png" width="500"/> </div>


**Differential Privacy Training Performance**

Comparison of the accuracy of the proposed model with and without Differential Privacy.


<div align="center"> <img src="differential_privacy.png" width="500"/> </div>

**Federated Learning Training Progress**

Accuracy plot over multiple federated learning rounds.

<div align="center"> <img src="Federated_Learning.png" width="500"/> </div>


## Notebook Implementation

The entire implementation is available in the following notebook:

`Fraud_Detection_from_kagglee2.ipynb`

The notebook includes:

- Data preprocessing and normalization
- GAN-based synthetic data generation
- Differential Privacy-based training
- Federated learning simulation

## Technologies Used

The project was built with the following technologies:

- Python
- Pandas
- NumPy
- PyTorch
- Opacus (Differential Privacy)
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Conclusion

The proposed project demonstrates how to effectively implement various privacy-preserving machine learning approaches in fraud detection scenarios with sensitive financial information.With the help of various machine learning approaches such as:

- Synthetic Data Generation
- Differential Privacy
- Federated Learning

it is possible to develop effective fraud detection models with guaranteed data privacy.






































