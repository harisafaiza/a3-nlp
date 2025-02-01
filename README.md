



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
