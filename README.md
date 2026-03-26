# 🔮 Next Word Prediction using LSTM

## 📌 Project Description

This project builds a **Next Word Prediction Model** using Deep Learning.
Given a sequence of words, the model predicts the most probable next word — similar to how smartphone keyboards suggest the next word while typing.

The model is trained on a text dataset (Sherlock Holmes novel) and uses an **LSTM (Long Short-Term Memory)** neural network to learn language patterns.

---

## ✨ Features

* Predicts next word(s) based on input text
* Uses LSTM for sequence learning
* Trained on real-world text dataset
* Memory-optimized for Google Colab
* Beginner-friendly implementation

---

## 🛠️ Tech Stack

* **Python**
* **TensorFlow / Keras**
* **NumPy**
* **Google Colab**

---

## ⚙️ How It Works

The project follows these steps:

1. **Dataset Loading**

   * Text file is loaded and converted to lowercase

2. **Text Cleaning**

   * Punctuation is removed

3. **Tokenization**

   * Words are converted into numeric sequences

4. **Sequence Creation**

   * Input-output pairs are generated using n-grams

5. **Padding**

   * Sequences are padded to equal length

6. **Model Training**

   * LSTM model learns word patterns

7. **Prediction**

   * Given a sentence, the model predicts next word(s)

---

## 🚀 Installation & Setup

### 1. Open Google Colab

Go to: https://colab.research.google.com/

### 2. Upload Dataset

Upload the file:

```
1661-0.txt
```

### 3. Install Dependencies

```bash
pip install tensorflow
```

### 4. Run All Cells

Execute the notebook step-by-step.

---

## ▶️ Usage

Example:

```
Input:  sherlock holmes
Output: sherlock holmes was a very
```

You can change the input text and number of predicted words in the code.

---

## 🧩 Code Structure

* **Data Preprocessing**
  Loads dataset, cleans text, and tokenizes words

* **Sequence Generation**
  Creates training sequences

* **Model Building**
  Embedding + LSTM + Dense layers

* **Training**
  Model learns patterns from text

* **Prediction Function**
  Generates next words

---

## ⚡ Optimization Notes

To prevent memory crashes in Google Colab:

* Dataset size was limited
* Vocabulary size reduced (`num_words=5000`)
* Used `sparse_categorical_crossentropy` instead of one-hot encoding
* Reduced epochs and model size

These optimizations ensure smooth training even on limited RAM.

---

## 🔮 Future Improvements

* Use **GRU or Transformer models**
* Build a **web interface (Streamlit/Flask)**
* Deploy on **AWS (EC2 / Lambda)**
* Train on larger datasets for better accuracy

---

## 👤 Author

* Lfee Deshwal

---

## ⭐ Final Note

This project is a great starting point for understanding:

* Natural Language Processing (NLP)
* Sequence Models
* Deep Learning with LSTM

Feel free to improve and extend it 🚀



## ⚠️ Model Performance Note

The current implementation of this project is intentionally optimized to run efficiently on **Google Colab's limited memory environment**.

To prevent runtime crashes and ensure smooth execution, the following optimizations were applied:

* Reduced dataset size
* Limited vocabulary (`num_words=5000`)
* Restricted number of training sequences
* Used `sparse_categorical_crossentropy` instead of one-hot encoding
* Reduced model complexity and training epochs

### 📉 Impact on Accuracy

Due to these constraints, the model may show **lower prediction accuracy and less coherent outputs** compared to a fully trained large-scale model.

### 📈 Expected Performance with Scaling

If trained with:

* Full dataset
* Larger vocabulary
* More epochs
* Increased model size (LSTM units)

👉 The model performance and prediction quality will **significantly improve**, producing more accurate and context-aware results.

### 🎯 Key Takeaway

This project demonstrates the **complete pipeline of an NLP sequence model**, focusing on:

* Correct implementation
* Efficient resource usage
* Scalability for real-world deployment

The current version is a **lightweight prototype**, not a fully optimized production model.
