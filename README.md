# 🏏 Topic Modeling of Cricket Commentary  
### A Comparative LDA Analysis of T20 vs Test Match Narratives

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![NLP](https://img.shields.io/badge/NLP-Topic%20Modeling-green)
![LDA](https://img.shields.io/badge/Model-LDA-orange)
![Status](https://img.shields.io/badge/Project-Complete-success)

---

## 📖 Project Overview

This project applies **Latent Dirichlet Allocation (LDA)** to cricket match commentary transcripts to compare **thematic structures and narrative focus** between:

- **T20 cricket** (short-form, high-intensity)
- **Test cricket** (long-form, strategic)

By modeling commentary text as probabilistic topic distributions, the project explores how **game format influences language, emphasis, and storytelling**.

---

## 🎯 Objectives

- Extract dominant topics from cricket commentary using LDA
- Compare thematic distributions between T20 and Test formats
- Analyze linguistic differences driven by match duration and pacing
- Demonstrate end-to-end NLP workflow on real-world sports text data

---

## 🧠 Methodology

1. **Data Collection**
   - Commentary transcripts sourced from publicly available cricket coverage
   - Separate corpora for T20 and Test matches

2. **Preprocessing**
   - Tokenization
   - Stopword removal
   - Lemmatization
   - Bigram/trigram detection

3. **Modeling**
   - Latent Dirichlet Allocation (Gensim)
   - Topic coherence used for model selection

4. **Evaluation & Visualization**
   - Topic-word distributions
   - Inter-format topic comparison
   - Qualitative interpretation

Detailed methodology is available in [`docs/methodology.md`](docs/methodology.md).

---

## 📂 Repository Structure

```text
notebooks/   → Exploratory and modeling notebooks  
src/         → Reusable preprocessing and modeling code  
docs/        → Written analysis and documentation  
assets/      → Visualizations and diagrams  
