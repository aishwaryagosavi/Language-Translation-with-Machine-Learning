# English to French Language Translator

## Overview
A sequence-to-sequence (Seq2Seq) deep learning model that translates 
English text to French, complete with a desktop GUI application 
built using Tkinter.

## What Makes This Project Different
This is not just a notebook — it is a fully functional desktop 
application. Users type English text into the GUI and receive 
French translations in real time using a trained LSTM model.

## How It Works
1. Trained a Seq2Seq LSTM model on 10,000 English-French sentence pairs
2. Model uses an encoder-decoder architecture with 256 hidden dimensions
3. Characters are encoded using bag-of-characters representation
4. Trained model is saved and loaded for inference
5. GUI built with Tkinter allows real-time translation

## Model Architecture
- Encoder LSTM — reads English input character by character
  and compresses it into a context vector (hidden + cell state)
- Decoder LSTM — takes the context vector and generates
  French output character by character
- Dense output layer with softmax activation over French characters

## Why Seq2Seq LSTM?
Translation is a sequence problem — the input and output are both 
sequences of different lengths. LSTM handles th
