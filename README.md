# 🤖📄 Resume-Job Matcher AI (SpaCy + Flutter)

An intelligent **AI-based Resume and Job Description Matcher** built using a **SpaCy pre-trained model**, fine-tuned on a custom dataset for semantic similarity, and fully integrated with a **Flutter mobile application** for real-time matching.

---

## 🔍 Overview

This project leverages natural language processing to evaluate and score the match between resumes and job descriptions. The model returns a similarity score (0–100), helping recruiters or job-seekers understand fit at a glance.

---

## 🛠️ Tech Stack

| Layer           | Technology Used           |
|----------------|---------------------------|
| NLP Model       | `SpaCy` (pre-trained model fine-tuned on custom data) |
| Training Engine | PyTorch + SpaCy Pipelines |
| Score Metric    | Custom regression (0–100) + mAP Evaluation |
| Frontend        | Flutter Mobile App        |
| Integration     | Python backend with `.pth` model export |

---

## 📦 Features

- ✨ Fine-tuned `SpaCy` Transformer pipeline for semantic understanding
- 🧠 Learns semantic similarity between resumes and job descriptions
- 📱 Integrated with Flutter frontend for real-time user feedback
- 📈 Shows training progress, rows processed, and mAP score per epoch
- 🔁 Supports retraining on new datasets (continual learning)

