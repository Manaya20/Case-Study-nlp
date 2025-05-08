# 🎮 Real-Time QoS Optimization in Game Streaming using Sentiment Analysis and Deep Learning

This project addresses the challenge of maintaining consistent Quality of Service (QoS) in live video game streaming platforms like Twitch and YouTube Gaming. We combine deep learning and sentiment analysis to create a data-driven, adaptive QoS management system that adjusts based on user feedback and engagement.

---

## 📌 Problem Statement

As live game streaming grows, platforms face real-time challenges like fluctuating network conditions, varying video quality, and inconsistent user engagement. Traditional QoS methods are reactive and lack personalization. This project proposes a deep learning-based approach that leverages BERT-based sentiment analysis and a neural network classifier for user satisfaction prediction and real-time QoS adjustment.

---

## 🚀 Solution Overview

Our system integrates:
- 🎯 Sentiment Analysis using BERT to interpret user feedback.
- 🧠 Deep Neural Network (DNN) for classifying user satisfaction from QoS metrics.
- ⚙️ Real-time QoS Action Recommendations (e.g., adjust bitrate, resolution).

---

## 🛠️ Technologies Used

- Python 🐍
- PyTorch 🔥
- Transformers (HuggingFace) 🤗
- Pandas, NumPy, Scikit-learn
- Matplotlib / Seaborn (for visualization)
- Jupyter Notebook / Google Colab

---

## 📊 Dataset Features

- Bitrate
- Framerate
- Dropped Frames
- Sentiment Score (Extracted via BERT from user comments)
- MOS (Mean Opinion Score)

---

## 🧠 Model Architecture

- Sentiment Classifier: Pretrained BERT → Sentiment Score
- Satisfaction Classifier: DNN
  - Input: Bitrate, Framerate, Dropped Frames, Sentiment
  - Hidden Layers: 2 (ReLU activations)
  - Output: 3 Classes (Low, Medium, High QoS satisfaction)
- Loss Function: CrossEntropyLoss
- Optimizer: Adam

---

## 🧪 Results

- ✅ Accuracy: 97.73% on Test Set
- ✅ Real-time QoS suggestions based on model output
- Sample Output:

| Sentiment | MOS | QoS Action Recommendation           |
|-----------|-----|-------------------------------------|
|     3     |  3  | Adjust bitrate or buffer            |
|     5     |  5  | Maintain current QoS                |
|     2     |  2  | Reduce resolution or switch server  |

---

