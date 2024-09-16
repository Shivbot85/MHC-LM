# Fine-Tuning ESM2 for MHC Peptide Binding Predictions

## Project Overview
This project focuses on fine-tuning the [ESM2](https://github.com/facebookresearch/esm) model, a state-of-the-art Protein Language Model (PLM), to improve predictions of MHC peptide binding. The project implements multiple fine-tuning techniques, including Transfer Learning, Low-Rank Adaptation (LoRA), and Contrastive Learning, to evaluate their effectiveness on the task of predicting MHC peptide binding affinities. The fine-tuned models are compared with the base ESM2 model and domain-adapted versions to assess performance improvements.

## Project Abbreviation
**MHC LLM**

## Author
**Shivaskar Naidoo**

## Supervisor
**Jan Buys**

## Goals and Objectives
- **Primary Objective:** Evaluate the effectiveness of different fine-tuning strategies (Transfer Learning, LoRA, and Contrastive Learning) in improving the predictive performance of the ESM2 model for MHC peptide binding predictions.
- **Secondary Objective:** Analyze the role of domain adaptation in enhancing model performance for this specific task.

## Key Features
- **Transfer Learning:** Adapts the ESM2 model to MHC peptide binding by adding task-specific layers.
- **Low-Rank Adaptation (LoRA):** Reduces the computational cost of fine-tuning by updating a small subset of model parameters.
- **Contrastive Learning:** Enhances the model's ability to distinguish between binding and non-binding peptides by learning from paired examples.

## Dataset
The data for this project is sourced from [NetMHCpan](http://www.cbs.dtu.dk/services/NetMHCpan/), a widely used tool for predicting peptide-MHC binding. The dataset consists of 30,000 MHC-peptide pairs, including their binding affinity scores.

## System Requirements
- **Hardware:** UCT’s high-performance computing cluster with Nvidia A100 GPUs.
- **Software:**
  - Python 3.8+
  - PyTorch
  - HuggingFace Transformers
  - Scikit-learn
  - Optuna (for hyperparameter optimization)

## Installation
To set up the environment for this project, clone this repository and install the required dependencies.

## Modals 
All trained Modals are freely available on my hugging account 
Username - Shivaskar

## Run instructions 
Running Instructions
Before running any code, ensure all data files are placed in a folder named data within your Google Colab or local environment.
1. Run Finetuning code
2. Run Domain Adaptation code 

```bash
git clone https://github.com/Shivbot85/MHC-LM.git
cd MHC-LM
pip install -r Requirements.txt

