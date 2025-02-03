https://github.com/harisafaiza/a3-nlp/blob/main/a3-nlp.mov

This is the screen recording of the website application.

📊 Attention Mechanism Performance Analysis

This project implements a Sequence-to-Sequence (Seq2Seq) translation model using three different attention mechanisms:

General Attention
Multiplicative Attention
Additive Attention
The table below presents a comparison of Training Loss, Training Perplexity (PPL), Validation Loss, and Validation PPL for each attention type after training.

📋 Performance Metrics Table


<img width="717" alt="table" src="https://github.com/user-attachments/assets/d325ab78-bf82-43e9-a945-f86efbaef55a" />


📊 Insights & Observations
🔹 Additive Attention achieves the lowest Training & Validation Loss and the best Perplexity (PPL), making it the most effective.

🔹 Multiplicative Attention performs slightly worse than Additive Attention but is computationally more efficient.

🔹 General Attention has the highest loss and PPL, making it the least effective attention mechanism.

🛠️ How These Metrics Were Calculated
Training Loss → Computed using Cross-Entropy Loss during model training.
Perplexity (PPL) → Calculated as:
P
P
L
=
e
Loss
PPL=e 
Loss
 
Validation Loss → Evaluated on a separate test dataset after training.

You can now view your Streamlit app in your browser.

  Local URL: http://localhost:8501
  Network URL: http://192.168.1.7:8501

  For better performance, install the Watchdog module:

  $ xcode-select --install
  $ pip install watchdog



1. Jupyter Notebooks

MT_Attention.ipynb
*  Implements a Sequence-to-Sequence (Seq2Seq) model with Attention using LSTMs.
*  Explores different types of attention mechanisms:
*  General Attention
*  Multiplicative Attention
*  Additive Attention
*  Includes model training, evaluation, and visualization of attention maps.


MT_Transformer.ipynb
*  Implements a Transformer-based Machine Translation model using the T5 model.
*  Fine-tunes the t5-small model for translation.
*  Includes training, inference, and comparison with the LSTM model.

2. Web Application

app.py
* A Streamlit-based web application for real-time machine translation.
* Users enter text, and the model generates a translation.
* Uses T5 Transformer for inference.

Model Architecture

The core of the model is based on the Transformer architecture, which uses the following key components:

Multi-Head Attention: Helps the model focus on different parts of the input sequence simultaneously, capturing different aspects of the sentence.
Positional Encoding: Adds information about the position of words in the sequence, crucial for handling sequential data.
Encoder-Decoder Structure: The encoder processes the input sequence, and the decoder generates the translated sequence, with attention mechanisms connecting them.
The model's attention mechanism allows it to handle long-range dependencies and improve translation quality significantly compared to traditional models like RNNs and LSTMs.
