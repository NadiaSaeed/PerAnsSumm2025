🚀 Medifact at PerAnsSumm 2025: Leveraging Lightweight Models for Perspective-Specific Summarization of Clinical Q & A Forums

📌 Overview

This repository contains the implementation of a hybrid NLP pipeline that classifies perspectives in multi-perspective answers and generates concise summaries. The workflow integrates:

🔹 Snorkel-based Weak Supervision – Heuristic rule-based labeling functions.

🔹 SVM Classifier – Trained on labeled spans for perspective prediction.

🔹 Zero-Shot Learning (ZSL) – Used when prior methods abstain.

🔹 Extractive & Abstractive Summarization – Combining BART (extractive) and Pegasus (abstractive) for refined summaries.

🔬 Methodology

Our approach consists of two key tasks:

1️⃣ Perspective Classification

Input: Clinical questions + multi-perspective answers.
Processing: Tokenization, feature extraction, and classification.

Classification Pipeline:

✅ Snorkel Labeling Functions (Rule-based labeling).

✅ SVM Classifier (Machine learning-based).

✅ Zero-Shot Model (Transformer-based fallback).

Output: Labeled text spans categorized into perspectives.

2️⃣ Perspective-Aware Summarization

Input: Classified text spans.

Summarization Pipeline:

✂️ Extractive Summarization (BART extracts key sentences).

✍️ Abstractive Summarization (Pegasus generates fluent summaries).

🔗 Contextual Integration (Summaries linked to the original question).

Output: Structured JSON summaries ready for decision-making.
