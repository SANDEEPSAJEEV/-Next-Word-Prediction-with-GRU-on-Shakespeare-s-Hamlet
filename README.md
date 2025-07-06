# 📘 Next Word Prediction with GRU on Shakespeare's Hamlet

This project implements a **GRU-based neural network** to perform **next word prediction** on Shakespeare's *Hamlet*. It also compares the performance of GRU with an LSTM-based architecture on the same dataset. The model learns language structure and predicts the next word in a sequence, demonstrating deep learning’s power in natural language generation.

---

## 🎯 Objective

To explore and evaluate the effectiveness of **Gated Recurrent Units (GRU)** for language modeling and predictive text generation, and compare it with LSTM on the same task and dataset.

---

## 🧠 Highlights

- Trained on Shakespeare’s *Hamlet* corpus from the NLTK Gutenberg dataset
- Uses GRU-based sequence model with embedding and dropout layers
- Performs next-word prediction given an input text sequence
- Compares GRU performance with LSTM-based model (accuracy, training time)

---

## 🧾 Project Structure


---

## ⚙️ Model Architecture

- **Embedding Layer** – Converts words to dense vectors
- **GRU Layer** – Captures sequential dependencies in text
- **Dropout Layer** – Prevents overfitting
- **Dense Output Layer** – Softmax over vocabulary for next word prediction

---

## 📈 Performance Summary

| Metric             | GRU Model | LSTM Model |
|--------------------|-----------|------------|
| Training Accuracy  | ~XX%      | ~YY%       |
| Validation Accuracy| ~XX%      | ~YY%       |
| Training Time      | Shorter   | Longer     |
| Prediction Quality | Slightly Lower | Better |

> _LSTM showed better contextual accuracy, while GRU converged faster._

---

## 🧪 Sample Usage

```python
input_text = "To be or"
next_word = predict_next_word(gru_model, tokenizer, input_text, max_sequence_len)
print(f"Next word: {next_word}")
