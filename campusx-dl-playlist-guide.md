# CampusX "100 Days of Deep Learning" — AI Engineering Watch Guide

Playlist: https://youtube.com/playlist?list=PLKnIA16_RmvYuZauWaPlRTC54KxSNLtNn
(84 videos total, Hindi-English, by Nitish Singh)

**Context:** This playlist was built for people becoming *deep learning practitioners/researchers* — it goes deep into ANN math, CNN internals, RNN backprop derivations, and every optimizer variant. If your goal is **AI engineering** (building products with LLMs — RAG, agents, fine-tuning, APIs), you need the *concepts*, not every derivation. Below is the full list with a priority tag.

Legend: 🟢 Watch — 🟡 Skim/Optional — 🔴 Skip for AI engineering path

---

## Block 1: Foundations (Day 1–14) — Perceptrons & ANN basics
| Day | Title | Priority |
|---|---|---|
| 1 | Course Announcement | 🔴 Skip (no content) |
| 2 | What is Deep Learning? DL vs ML | 🟢 Watch |
| 3 | Types of Neural Networks, History, Applications | 🟢 Watch |
| 4 | What is a Perceptron? Perceptron vs Neuron | 🟢 Watch |
| 5 | Perceptron Trick — how to train a Perceptron | 🟡 Skim |
| 6 | Perceptron Loss Function, Hinge Loss, BCE, Sigmoid | 🟢 Watch |
| 7 | Problem with Perceptron | 🟡 Skim |
| 8 | MLP Notation | 🟡 Skim (only if next video confuses you) |
| 9 | Multi Layer Perceptron — MLP Intuition | 🟢 Watch |
| 10 | Forward Propagation | 🟢 Watch |
| 11 | Customer Churn Prediction using ANN (Keras) | 🟢 Watch (first real code) |
| 12 | Digit Classification using ANN (MNIST) | 🟡 Skim — same pattern as Day 11 |
| 13 | Graduate Admission Prediction using ANN | 🔴 Skip — repeat pattern |
| 14 | Loss Functions in Deep Learning | 🟢 Watch |

## Block 2: Backprop & Training Mechanics (Day 15–23)
| Day | Title | Priority |
|---|---|---|
| 15 | Backpropagation Part 1 — The What | 🟢 Watch |
| 16 | Backpropagation Part 2 — The How | 🟡 Skim — watch if you want the math |
| 17 | Backpropagation Part 3 — The Why | 🔴 Skip unless you love calculus |
| 18 | MLP Memoization | 🔴 Skip — implementation detail |
| 19 | Gradient Descent: Batch vs Stochastic vs Mini-batch | 🟢 Watch |
| 20 | Vanishing/Exploding Gradient Problem | 🟢 Watch — important intuition |
| 21 | How to Improve Performance of a Neural Network | 🟢 Watch — good roadmap overview |
| 22 | Early Stopping | 🟡 Skim |
| 23 | Data/Feature Scaling in ANN | 🟡 Skim (you likely know this from ML) |

## Block 3: Regularization, Activations, Init, Optimizers (Day 24–39)
This block is the most "skippable" for an AI engineer — it's classic DL tuning theory, largely abstracted away by modern frameworks/libraries (HuggingFace, PyTorch Lightning) and less relevant once you move to LLM-based work.

| Day | Title | Priority |
|---|---|---|
| 24 | Dropout Layer — concept | 🟢 Watch |
| 25 | Dropout — Code example | 🔴 Skip |
| 26 | L1/L2 Regularization, Weight Decay | 🟡 Skim |
| 27 | Activation Functions: Sigmoid, Tanh, ReLU | 🟢 Watch — need this |
| 28 | ReLU Variants (Leaky/Parametric/ELU/SELU) | 🔴 Skip — rarely used directly today |
| 29 | Weight Initialization — what NOT to do | 🟡 Skim |
| 30 | Xavier/Glorot & He Initialization | 🔴 Skip — you'll never hand-pick this |
| 31 | Batch Normalization | 🟢 Watch — concept shows up everywhere |
| 32 | Optimizers Part 1 (intro) | 🟢 Watch |
| 33 | Exponentially Weighted Moving Average | 🔴 Skip — just math prereq for next 2 |
| 34 | SGD with Momentum | 🔴 Skip |
| 35 | Nesterov Accelerated Gradient | 🔴 Skip |
| 36 | AdaGrad | 🔴 Skip |
| 37 | RMSProp | 🔴 Skip |
| 38 | **Adam Optimizer** | 🟢 Watch — this is the one optimizer you actually need to understand |
| 39 | Keras Tuner — hyperparameter tuning | 🔴 Skip |

## Block 4: CNNs (Day 40–54)
Skip most of the deep internals unless you're going into computer vision specifically. AI engineering today is overwhelmingly text/LLM focused; CNNs matter mainly for multimodal context.

| Day | Title | Priority |
|---|---|---|
| 40 | What is CNN — Intuition | 🟢 Watch |
| 41 | CNN vs Visual Cortex, Cat Experiment (history) | 🔴 Skip |
| 42 | Convolution Operation | 🟢 Watch |
| 43 | Padding & Strides | 🟡 Skim |
| 44 | Pooling Layer / MaxPooling | 🟡 Skim |
| 45 | LeNet-5 Architecture | 🔴 Skip |
| 46 | CNN vs ANN comparison | 🔴 Skip |
| 47 | Backprop in CNN Part 1 | 🔴 Skip |
| 48 | CNN Backprop Part 2 | 🔴 Skip |
| 49 | Cat vs Dog Classification Project | 🟡 Skim — decent applied example |
| 50 | Data Augmentation | 🟡 Skim |
| 51 | Pretrained Models, ImageNet, ILSVRC | 🟢 Watch — transfer learning concept matters |
| 52 | Visualizing CNN Filters/Feature Maps | 🔴 Skip |
| 53 | Transfer Learning: Fine-tuning vs Feature Extraction | 🟢 Watch — this concept reappears with LLMs |
| 54 | Keras Functional API | 🔴 Skip — framework-specific plumbing |

## Block 5: RNNs / LSTMs / GRUs (Day 55–66)
Mostly historical context now — sequence modeling has moved to Transformers. Watch just enough to understand *why* Transformers were invented (this is genuinely useful context for AI engineering), skip deep RNN training mechanics.

| Day | Title | Priority |
|---|---|---|
| 55 | Why RNNs are needed — RNN vs ANN | 🟢 Watch |
| 56 | RNN Forward Propagation / Architecture | 🟡 Skim |
| 57 | RNN Sentiment Analysis (Keras code) | 🔴 Skip |
| 58 | Types of RNN (many-to-many etc.) | 🟡 Skim |
| 59 | Backpropagation Through Time | 🔴 Skip |
| 60 | Problems with RNN | 🟢 Watch — sets up why LSTM/attention exist |
| 61 | LSTM Part 1 — The What | 🟢 Watch |
| 62 | LSTM Architecture Part 2 — The How | 🟡 Skim |
| 63 | LSTM Part 3 — Next Word Predictor | 🔴 Skip |
| 64 | GRU | 🔴 Skip |
| 65 | Deep/Stacked RNNs/LSTMs/GRUs | 🔴 Skip |
| 66 | Bidirectional RNN/LSTM/GRU | 🔴 Skip |

## Block 6: LLM History, Attention & Transformers (Day 67–84) — THE CORE FOR AI ENGINEERING
**This entire block is essential.** This is the part of the playlist that's directly relevant to modern AI engineering — everything from GPT to Claude is built on these ideas. Watch all of these in order, don't skip.

| Day | Title | Priority |
|---|---|---|
| 67 | History of LLMs — From LSTMs to ChatGPT | 🟢 Watch |
| 68 | Encoder-Decoder / Seq2Seq Architecture | 🟢 Watch |
| 69 | Attention Mechanism (in 1 video) | 🟢 Watch |
| 70 | Bahdanau vs Luong Attention | 🟡 Skim — nice to know, skippable if short on time |
| 71 | Introduction to Transformers | 🟢 Watch |
| 72 | Self Attention — Part 2 | 🟢 Watch |
| 73 | Self Attention with Code | 🟢 Watch |
| 74 | Scaled Dot Product Attention — why scale? | 🟢 Watch |
| 75 | Self Attention Geometric Intuition | 🟡 Skim — good if visual learner |
| 76 | Self Attention vs Luong Attention (deep dive) | 🔴 Skip — redundant with 69/70 |
| 77 | Multi-head Attention | 🟢 Watch |
| 78 | Positional Encoding | 🟢 Watch |
| 79 | Layer Normalization vs Batch Norm | 🟢 Watch |
| 80 | Transformer Architecture Part 1 — Encoder | 🟢 Watch |
| 81 | Masked Self Attention / Masked Multi-head | 🟢 Watch |
| 82 | Cross Attention | 🟢 Watch |
| 83 | Transformer Decoder Architecture | 🟢 Watch |
| 84 | Transformer Inference | 🟢 Watch |

---

## TL;DR — fastest path to AI engineering readiness
If you're short on time, here's the minimum viable path (~35 videos out of 84):

**Foundations:** 2, 3, 4, 6, 9, 10, 11, 14
**Training mechanics:** 15, 19, 20, 21
**Regularization essentials:** 24, 27, 31, 32, 38
**CNN (just enough):** 40, 42, 51, 53
**RNN (just enough context):** 55, 60, 61
**Attention & Transformers (all of it):** 67–69, 71–75, 77–84

## What to do after this playlist
The playlist stops at "Transformer Inference" (Day 84) — it doesn't cover the actual AI engineering stack. CampusX has follow-up playlists that pick up exactly where this leaves off:
- **Natural Language Processing (NLP)** — tokenization, embeddings, word2vec, text preprocessing
- **Practical Deep Learning using PyTorch** — since this playlist uses Keras/TensorFlow, and most modern AI engineering (HuggingFace, fine-tuning) is PyTorch-based
- **Model Context Protocol (MCP)** and **Agentic AI using LangGraph** — the actual "AI engineering" layer: building agents, tool use, RAG pipelines

Those are the ones that turn "I understand transformers" into "I can build LLM applications."
