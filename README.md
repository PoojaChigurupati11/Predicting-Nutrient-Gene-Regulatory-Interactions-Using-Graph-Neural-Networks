# Predicting-Nutrient-Gene-Regulatory-Interactions-Using-Graph-Neural-Networks

# 🧬 Predicting Nutrient–Gene Regulatory Interactions using Graph Neural Networks

This project leverages **Graph Neural Networks (GNNs)** to predict novel regulatory interactions between nutrients and human genes. By modeling the biological data as a bipartite graph, we train a GCN-based link prediction model to uncover potential relationships that have not yet been experimentally validated.

## 🔍 Problem Statement

Certain nutrients (e.g., vitamins, minerals, bioactives) regulate gene expression. But most nutrient–gene interactions remain unknown due to experimental constraints. Can we **predict these hidden regulatory links** computationally?

### Goal
Treat this as a **link prediction problem**:
- **Nodes**: Nutrients and genes
- **Edges**: Known regulatory interactions
- **Objective**: Predict new (unseen) nutrient–gene links

---

## 📁 Datasets Used

1. **CTD (Comparative Toxicogenomics Database)**  
   Known chemical-gene interactions  
   🔗 https://ctdbase.org/downloads/

2. **HMDB (Human Metabolome Database)**  
   Used to filter for nutrients only  
   🔗 https://hmdb.ca/downloads

3. **BioMart / Ensembl Gene Metadata**  
   Human gene metadata (symbols, chromosomes)  
   🔗 https://useast.ensembl.org/index.html

---

## 🧠 Model Architecture

- **Graph Convolutional Network (GCN)** for node embedding
- **MLP-based link predictor** to estimate interaction probability
- Framework: PyTorch Geometric

---

## ✨ Features

- Link prediction on bipartite biological graph
- Model trained on known nutrient–gene interactions
- Top-K prediction of **novel regulatory pairs**
- ROC-AUC: **0.9882**, Test Accuracy: **95.2%**

---

