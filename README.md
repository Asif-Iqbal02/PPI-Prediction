# Protein–Protein Interaction (PPI) Prediction Using Auto-Covariance and GCN

## Overview

This project explores protein–protein interaction (PPI) prediction using sequence-based feature extraction and graph neural networks. It uses Auto-Covariance (AC) features to represent protein sequences and a Graph Convolutional Network (GCN) to learn from graph-structured protein interaction data.

The goal is to develop a machine-learning workflow that can help predict potential interactions between proteins.

## Objectives

- Process protein–protein interaction data.
- Retrieve and prepare protein sequence information.
- Extract sequence-based features using Auto-Covariance.
- Represent proteins and their relationships using a graph.
- Train and evaluate a GCN-based prediction model.
- Examine model predictions using appropriate evaluation metrics.

## Methodology

1. **Data preparation:** Load and filter protein interaction records.
2. **Protein sequence processing:** Map protein identifiers to available protein sequences and prepare the sequence data.
3. **Feature extraction:** Represent protein sequences using Auto-Covariance features based on selected sequence properties.
4. **Graph construction:** Represent proteins as nodes and known interactions as edges.
5. **Model training:** Apply a Graph Convolutional Network to learn representations from the graph.
6. **Evaluation:** Evaluate predictions on held-out data using suitable metrics.

## Technologies

- Python
- Google Colab
- NumPy and pandas
- PyTorch
- PyTorch Geometric
- NetworkX
- BioGRID interaction data
- UniProt protein sequence data

## Repository Contents

- `PPI_GCN_Training_and_Evaluation.ipynb` — notebook containing the project's implementation, training workflow, and evaluation code.

## How to Run

1. Open the notebook in Google Colab.
2. Ensure the required Python libraries are installed.
3. Configure access to the required interaction data and protein sequences.
4. Run the notebook cells in order.
5. Review the training output and evaluation results.

## Evaluation and Reproducibility

Model performance should be assessed on data held out from training. Negative interaction samples, data splitting, and graph construction should be handled carefully to prevent information leakage. Reported metrics should reflect the actual evaluation procedure.

## Future Work

- Improve the physicochemical-property-based Auto-Covariance feature representation.
- Explore alternative graph neural network architectures.
- Evaluate on larger and more diverse datasets.
- Improve negative-sample selection and validation.
- Add visualizations and further evaluation metrics.

## Author

**Asif-Iqbal02**

## Disclaimer

This repository is an academic and experimental project. Predictions indicate potential interactions and should not be interpreted as experimental confirmation of protein interactions.
