# LLM Model Training

| Model Type                    | Uses                                  | Training Objective                 | Simple Example                                                     | Real-World Model Examples |
| ----------------------------- | ------------------------------------- | ---------------------------------- | ------------------------------------------------------------------ | ------------------------- |
| **Encoder-only**              | Classification (e.g., Sentiment, NER) | **Masked Language Modeling (MLM)** | Input: "The cat sat on the \[MASK]." <br> Target: "mat"            | BERT, RoBERTa             |
| **Decoder-only**              | Text generation, zero-shot tasks      | **Causal Language Modeling (CLM)** <br> Predicts next token | Input: "The cat sat on the" <br> Target: Predict next token: "mat" | GPT-2, GPT-3, BLOOM       |
| **Encoder-Decoder (Seq2Seq)** | Translation, Summarization, QA        | **Span Corruption**              | Input: "The cat \<x> on the \<y>." <br> Target: "\<x> sat \<y> mat"    | T5, BART                  |

## Training Goals

In short, the training goals are:
- Increse model size (parameters)
- Increase training data (tokens)
- Minimize token prediction loss (maximize the performance), more compute budget

But compute hardware resources and training period (time) might be constant in a real-life scenario. 

## Quick Intro to the Units
**1 petaFLOP/s:** 1,000,000,000,000,000 (one quadrillion) floating point operations per second. So 1 petaFLOP/s-day roughly requires 8 NVDIA V100 GPUs for 1 day or 2 A100 GPUs at full efficiency. 
GPT-3 (175B params) ≈ 3,700 PF/s-days.

## The Chinchilla Paper
Smaller models with more data can outperform larger models trained with too little data

| Model        | Params (B) | Tokens Trained (T) | Compute-Optimal? |
| ------------ | ---------- | ------------------ | ---------------- |
| Chinchilla   | 70         | 1.4                | ✅                |
| LLaMA        | 65         | 1.4                | ✅ (near-optimal) |
| GPT-3        | 175        | 0.3                | ❌                |
| BloombergGPT | 50         | ✓ compute-optimal  | ✅                |
