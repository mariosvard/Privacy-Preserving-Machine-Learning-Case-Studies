Classical Data Anonymization Methods
Overview

This project demonstrates and compares classical data anonymization techniques used to protect sensitive information in datasets. The goal is to examine how different privacy-preserving methods affect data utility while maintaining privacy.

The project analyzes three well-known anonymization techniques:

k-Anonymity

l-Diversity

t-Closeness

Using a healthcare dataset, the notebook applies these methods and evaluates their impact on data retention and utility.

Project Structure
.
├── classical_final.ipynb        # Main notebook containing the anonymization implementation
├── healthcare_data.xls          # Dataset used for the anonymization experiments
├── privacy_utility_plot.png     # Visualization of privacy–utility trade-off
└── README.md                    # Project documentation
Dataset

The dataset used in this project contains healthcare-related information. Sensitive attributes are anonymized using classical privacy-preserving techniques.

Typical attributes may include:

Age

Gender

Location

Medical condition

Other healthcare-related variables

These attributes are processed to ensure individuals cannot be easily re-identified.

Methods
k-Anonymity

k-Anonymity ensures that each record in the dataset is indistinguishable from at least k−1 other records based on quasi-identifiers.

Goal: Prevent re-identification by grouping similar records.

l-Diversity

l-Diversity extends k-anonymity by ensuring that sensitive attributes in each group have at least l well-represented values.

Goal: Prevent attribute disclosure attacks.

t-Closeness

t-Closeness improves privacy further by ensuring that the distribution of a sensitive attribute in any group is close to the distribution in the entire dataset.

Goal: Prevent inference attacks based on distribution differences.

Results

The project evaluates the trade-off between privacy protection and data utility.

Metrics analyzed include:

Retention Rate – percentage of original data preserved

Utility Score – how useful the anonymized data remains for analysis

The results are visualized in the privacy–utility plot, showing how each method balances privacy and usability.

Requirements

To run the notebook you will need:

Python 3.x

Jupyter Notebook

Required libraries:

pandas
numpy
matplotlib
openpyxl

Install them using:

pip install pandas numpy matplotlib openpyxl
How to Run

Clone or download the project.

Install the required dependencies.

Open the notebook:

jupyter notebook classical_final.ipynb

Run all cells to reproduce the anonymization results and visualization.

Purpose

This project is intended for educational purposes and demonstrates how classical privacy-preserving techniques can be applied to real datasets. It highlights the balance between protecting personal data and maintaining analytical value.