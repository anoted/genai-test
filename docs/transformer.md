[⬅ Back to Learning Methodology](../docs/learn.md)

### Transformer and Self-Attention Mechanism

The **Transformer** is a deep learning model introduced by *Vaswani et al. (2017)* in the paper ["Attention Is All You Need"](https://arxiv.org/abs/1706.03762). It is widely used for natural language processing (NLP) tasks and has influenced architectures like BERT and GPT.  

## Architecture  

The Transformer model is composed of an **encoder-decoder** structure:  

### 1. Encoder  
- Consists of **N** identical layers.  
- Each layer has:  
  - **Multi-Head Self-Attention**: Captures dependencies between words regardless of their position.  
  - **Feed-Forward Network (FFN)**: Applies non-linearity and feature transformation.  
  - **Layer Normalization & Residual Connections**: Stabilizes training.  

### 2. Decoder  
- Also consists of **N** identical layers, with components similar to the encoder.  
- Additional **Masked Multi-Head Self-Attention** prevents future tokens from influencing predictions.  
- Uses **Cross-Attention** to attend to encoder outputs.  

## Key Components  

### 1. Self-Attention  
Computes attention scores to weigh input tokens relative to each other. Defined as:  
\[
\text{Attention}(Q, K, V) = \text{softmax} \left( \frac{QK^T}{\sqrt{d_k}} \right) V
\]
where:  
- \( Q \) (Query), \( K \) (Key), and \( V \) (Value) are projected from input embeddings.  
- \( d_k \) is the dimensionality of \( K \).  

### 2. Multi-Head Attention  
- Uses multiple self-attention heads in parallel.  
- Captures different types of relationships in data.  

### 3. Positional Encoding  
- Since the Transformer lacks recurrence, positional encodings are added to input embeddings:  
\[
PE_{(pos, 2i)} = \sin\left(\frac{pos}{10000^{2i/d}}\right)
\]
\[
PE_{(pos, 2i+1)} = \cos\left(\frac{pos}{10000^{2i/d}}\right)
\]

## Advantages  
- **Parallelization**: Unlike RNNs, it processes entire sequences at once.  
- **Long-Range Dependencies**: Captures distant relationships efficiently.  
- **Scalability**: Enables training on large datasets.  

## Applications  
- Machine Translation (e.g., Google Translate)  
- Text Generation (e.g., GPT, BERT)  
- Protein Structure Prediction (e.g., AlphaFold)  
- Time-Series Forecasting  

## References  
- Vaswani, A., et al. (2017). "Attention Is All You Need." *NeurIPS* (https://arxiv.org/abs/1706.03762).



[⬅ Back to Learning Methodology](../docs/learn.md)