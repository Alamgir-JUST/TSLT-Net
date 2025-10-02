# A Novel Unified Lightweight Temporal-Spatial Transformer Approach for Intrusion Detection in Drone Networks

This repository contains the full implementation and experiments from the paper:

> **A Novel Unified Lightweight Temporal-Spatial Transformer Approach for Intrusion Detection in Drone Networks**  
> Tarun Kumar Biswas, Ashrafun Zannat, Waqas Ishtiaq, Md. Alamgir Hossain  
> [Scientific Reports – under review]

---

## 📂 Repository Structure

| File | Description |
|------|-------------|
| **Coding-01_Drone_IDS_TSLT_Net.ipynb** | Main notebook implementing the proposed **TSLT-Net** model: data preprocessing, feature reshaping, multi-head self-attention, training, evaluation, and result visualization (accuracy, loss curves, confusion matrices). |
| **Coding-02_Drone_IDS_1D_CNN_MLP_and_GRU.ipynb** | Baseline models: 1D-CNN, Multi-Layer Perceptron (MLP), and Gated Recurrent Unit (GRU). Includes training scripts, performance metrics (precision/recall/F1), and comparison plots. |
| **Coding-03_Drone_IDS_RNN.ipynb** | Additional recurrent baselines (SimpleRNN and LSTM). Shows training/validation curves, confusion matrices, and parameter count analysis. |

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/TSLT-Net.git
   cd TSLT-Net

## 🗄️ Dataset

> We use the ISOT Drone Anomaly Detection Dataset:
https://doi.org/10.1007/978-3-031-87499-4_12

> ~2.35M records (benign + multiple attack types)

> Preprocessing: median/mode imputation, z-score normalization, label encoding

> Train/test split: 80/20 stratified

## 📊 Key Results

   TSLT-Net:

   Accuracy 99.99% (multiclass) / 100% (binary)

   Only 9,722 parameters (~0.04 MB) — ideal for edge deployment

   Outperforms CNN, MLP, GRU, LSTM, and RNN in both performance and efficiency
