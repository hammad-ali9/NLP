# 📄🤖 Resume-Job Matcher AI (with Flutter Integration)

This project is an AI-powered Resume-Job Matching system that evaluates the compatibility between job descriptions and applicant resumes. Built using PyTorch and Hugging Face Transformers, and seamlessly integrated into a Flutter mobile application for end-user interaction.

---

## 🚀 Features

- 🧠 Fine-tuned Transformer-based model
- 📊 Trained using Mean Squared Error Loss & optimized with AdamW
- 📈 Evaluates match scores and returns a similarity score (0 to 100)
- 🔎 Semantic similarity using BERT-like model
- 📱 Integrated with a Flutter mobile app
- ✅ Displays model training progress, mAP scores, and row counts per epoch

---

## 🛠️ Tech Stack

| Component       | Technology             |
|----------------|------------------------|
| AI Model       | Hugging Face Transformers, PyTorch |
| Training       | MSE Loss, AdamW, StepLR scheduler |
| Evaluation     | mean Average Precision (mAP) |
| Frontend App   | Flutter (Dart)         |
| Integration    | PyTorch `.pth` model used in backend API or direct inference |

---

## 🧪 Model Training

- Dataset: Resume and job description pairs
- Labels: Match score from 0 to 100
- Training Epochs: 2+ (retrainable)
- Output: Trained `.pth` model

### Training Highlights:
- Batch-wise progress logging
- mAP calculation after each epoch
- Saved using: `torch.save(model.state_dict(), 'model.pth')`

---

## 🔁 Retraining Support

Yes! The `.pth` model retains past training.
To **continue training on a new dataset**, just load the weights:

```python
model.load_state_dict(torch.load('model.pth'))
model.train()
