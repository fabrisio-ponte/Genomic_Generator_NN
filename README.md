# Genomic Generator Neural Network

This repository contains implementations of neural network models for genomic sequence analysis. The models are designed to process DNA sequences and predict the next nucleotide or k-mer using Recurrent Neural Networks (RNNs) and attention mechanisms.

## Models

### 1. DNA RNN Model
This model uses an LSTM-based RNN to predict the next nucleotide in a DNA sequence. The DNA sequence is encoded into integers, and the model learns to predict the next character in the sequence.

#### Key Features:
- Input: DNA sequence (A, C, G, T).
- Output: Predicted next nucleotide.
- Architecture: Embedding layer, LSTM, and a fully connected layer.

#### Training:
- Loss: CrossEntropyLoss.
- Optimizer: Adam.
- Training data: 80% of the DNA sequence.
- Test data: 20% of the DNA sequence.

---

### 2. DNA (k-mer) RNN Model
This model processes DNA sequences as k-mers (subsequences of length `k`) and predicts using only RNN as layers

### 3. DNA (k-mer) RNN Model and Attention Mechanism
This model processes DNA sequences as k-mers (subsequences of length `k`) and predicts using RNN and Attention Mechanism as layers