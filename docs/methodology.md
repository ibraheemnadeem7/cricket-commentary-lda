# Methodology

This document describes the data collection, preprocessing, modeling, and evaluation steps used in this study.

---

## 1. Data Collection

Full-length international cricket match videos were collected from YouTube. Only **complete matches** were used to avoid bias introduced by highlight clips, which disproportionately feature high-action moments and exclude technical commentary.

Sources included official cricket boards such as:
- Windies Cricket
- Pakistan Cricket
- England & Wales Cricket Board
- T Sports

From these videos:
- 15 T20 matches
- 23 Test matches

were selected.

---

## 2. Transcript Extraction

Transcripts were manually extracted using **youtubetotranscript.com**.

Each match transcript was initially stored as a single unstructured text block. To improve modeling quality:
- Each match was stored as a **separate document**
- Large combined corpora were also created per format

---

## 3. Data Cleaning

To ensure linguistic relevance, the following were removed:
- Audience noise labels (e.g., `[Applause]`, `[Music]`, `[Laugh]`)
- Non-commentary artifacts

Final corpus sizes:
- **Test matches**: 582,057 words
- **T20 matches**: 297,397 words

---

## 4. Text Preprocessing

Preprocessing steps included:
- Lowercasing
- Tokenization
- Stopword removal
- Lemmatization
- Paragraph segmentation via custom Python scripts
- N-gram construction for cricket-specific phrases

---

## 5. Topic Modeling

Latent Dirichlet Allocation (LDA) was applied **separately** to each format.

Model parameters:
- **Test cricket**: 14 topics
- **T20 cricket**: 15 topics
- **Lambda (λ)**: 0.8

These values were selected to achieve well-separated and interpretable topics.

---

## 6. Evaluation

Topics were evaluated qualitatively by:
- Inspecting top words per topic
- Comparing thematic overlap and divergence
- Analyzing filler word presence and technical vocabulary usage

