<p align="center">
  <img src="https://img.shields.io/github/license/Azzam-Radman/Arabic-Singular-to-Plural-Conversion?style=flat-square" />
  <img src="https://img.shields.io/github/languages/top/Azzam-Radman/Arabic-Singular-to-Plural-Conversion?style=flat-square" />
  <img src="https://img.shields.io/badge/Model-BERT%2FTransformer-blue?style=flat-square" />
  <img src="https://img.shields.io/badge/Platform-Colab%2FKaggle-orange?style=flat-square" />
</p>

<h1 align="center">Arabic Singular-to-Plural Conversion</h1>

<p align="center">
  🔤 NLP model for converting Arabic singular words to their plural forms using Character-BERT and Transformer architectures.
</p>

---

## 🚀 Overview

This repository contains code, data, and models from our paper:

> **"Neural Arabic Singular-to-Plural Conversion with a Pre-trained Character-BERT and a Fused Transformer"**

Our research addresses the Morphological Inflection Generation (MIG) task proposed by [SIGMORPHON 2022](https://github.com/sigmorphon/2022InflectionST/blob/main/part2/README.md), focusing on Arabic—a morphologically rich language. We first pre-train an Arabic Character-BERT on a Masked Language Modeling (MLM) task, then incorporate it into two custom Transformer-based architectures.

## 🧠 Key Features

- **Arabic Character-BERT** pre-trained from scratch
- **Two novel architectures**: Fused and Direct
- **Colab and Kaggle ready** notebooks
- Minimal setup, fully reproducible
- Data-driven and modular design

---

## 📂 Table of Contents

1. [Datasets](#1-datasets)
2. [Model Architectures](#2-model-architectures)
3. [Getting Started](#3-getting-started)
4. [License](#4-license)

---

## 1. Datasets

We use two datasets:

- **Pre-training Dataset**  
  Cleaned Arabic Wikipedia corpus from [Abed Khooli on Kaggle](https://www.kaggle.com/datasets/abedkhooli/arabic-bert-corpus/discussion/129597), containing over **1.1 million unique Arabic words**.

- **Downstream MIG Dataset**  
  Provided by [SIGMORPHON 2022](https://github.com/sigmorphon/2022InflectionST/tree/main/part2) organizers, containing singular-to-plural pairs in context.

---

## 2. Model Architectures

We introduce two different Transformer-based approaches to plural conversion:

### 🔁 Fused Architecture

- Embeddings from Character-BERT are **fused** into both the encoder and decoder of a Transformer.
- Performs better on morphologically complex forms.

<p align="center">
  <img src="/figures/Computational%20Linguistics%20Model-Fused.png" alt="Fused Architecture" width="1000"/>
</p>

### ➡️ Direct Architecture

- Character-BERT is used **directly** as the encoder in the Transformer pipeline.
- Lightweight and faster in training.

<p align="center">
  <img src="/figures/Computational%20Linguistics%20Model-Direct.png" alt="Direct Architecture" width="600"/>
</p>

---

## 3. Getting Started

### ✅ Requirements

- Python 3.x
- Google Colab (recommended)
- Kaggle (for Notebook 2)

### 📘 Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/Azzam-Radman/Arabic-Singular-to-Plural-Conversion.git
   ```

2. Open the notebooks in Google Colab or Kaggle Kernels.

3. Run cells sequentially—no additional setup required.

⚠️ Some paths may be hard-coded for Colab/Kaggle. If running locally, adjust file paths accordingly.

## 4. License
This project is licensed under the MIT License.

## 📬 Citation
If you use this work, please cite our [paper](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=QUGRpw4AAAAJ&citation_for_view=QUGRpw4AAAAJ:d1gkVwhDpl0C).

## 🤝 Acknowledgments
[SIGMORPHON 2022](https://sigmorphon.github.io/sharedtasks/2022/)

[Abed Khooli](https://github.com/abedkhooli) for the Arabic BERT corpus
