# Fine-tuning DistilBERT for Emotion Detection

## 👥 Team Information

**Course:** Deep Learning  
**Institution:** Telkom University  

| Name | NIM |
| :--- | :--- |
| **Fasya Burhanis Syauqi** | 1103223054 |
| **Muhammad Muhammad Farhan** | 11032320187 |

---

## 🎯 Purpose

This repository contains the implementation of **Task 2: Multi-Label Classification**.

The objective is to fine-tune a pre-trained **DistilBERT** model to detect human emotions in text. Unlike standard classification, a single text input here can be associated with multiple emotions simultaneously.

## 🔍 Project Overview

### The Task: Multi-Label Classification
We utilize the **GoEmotions** dataset to identify subtle emotions in Reddit comments. The model must output a probability vector where multiple classes can be valid (output > threshold).

### The Model: DistilBERT Base Uncased
* **Architecture:** Distilled version of BERT (Transformer Encoder).
* **Approach:** We configure the model with `problem_type="multi_label_classification"` which utilizes **BCEWithLogitsLoss** for optimization.

### The Dataset: GoEmotions (Simplified)
* **Input:** A raw text comment.
* **Output:** Binary vector representing 28 possible emotions (e.g., Admiration, Joy, Anger, Neutral, etc.).

---

## 📊 Technical Approach

### Model Configuration
* **Base Model:** `distilbert-base-uncased`
* **Tokenizer:** DistilBertTokenizer
* **Framework:** PyTorch & Hugging Face Transformers

### Training Configuration
* **Batch Size:** 32
* **Learning Rate:** 2e-5
* **Epochs:** 3
* **Optimizer:** AdamW

### Results
The model achieved a Micro F1-Score and Accuracy of approximately **96.9%** on the validation set.
