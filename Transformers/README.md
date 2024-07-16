# Transformers Assignment

This folder contains the assignment on exploring Encoder-Decoder based Transformer Models. The objective is to understand the architecture, working principles, and innovations introduced by transformer models in Natural Language Processing (NLP).

## Files

- **Transformer_Assignment_Devesh.ipynb:** Jupyter Notebook with the complete code and analysis.
- **Transformer_Presentation.pptx:** PowerPoint presentation summarizing the findings.

## Background

Transformers have revolutionized NLP, particularly in Natural Language Generation (NLG). They focus on converting data into natural language, handling tasks like summarization and translation. Early approaches using Deep Neural Networks (DNNs) and Recurrent Neural Networks (RNNs) faced limitations, such as the vanishing gradient problem and inefficiency in parallel processing.

## Encoder-Decoder Architecture for Transformers

### Introduction to the Transformer Model

- Introduced by the "Attention is All You Need" paper by Vaswani et al.
- Departs from recurrent structures to stacks of residual attention blocks, enhancing efficiency through parallelization.

### How Transformer-based Encoder-Decoder Models Work

- **Encoder Overview:** Processes input tokens into a sequence of hidden states, creating a contextualized representation.
- **Decoder's Role:** Predicts the next word in the sequence using the encoded input and previously generated words.

## Encoder Architecture Explained

- **Stacked Encoder Blocks:** Multiple identical layers forming the encoder part of the model.
- **Residual Connections:** Prevent vanishing gradient problems.
- **Self-Attention Mechanism:** Understands context and relationships between words.
- **Normalization and Feed-Forward Networks:** Stabilize learning and transform data within each encoder block.

## Understanding the Self-Attention Mechanism

- **Purpose:** Understands context and relationships between words.
- **Input Transformation:** Transforms input into queries (Q), keys (K), and values (V).
- **Self-Attention Scores:** Weights on values determine relevance.
- **Output Generation:** Produces a continuous representation of the input text.

## Decoder Architecture Explained

- **Stacked Decoder Blocks:** Generate the output sequence.
- **Language Model (LM) Head:** Predicts the next token in the sequence.
- **Uni-directional Self-Attention:** Prevents attending to future positions.
- **Cross-Attention Mechanism:** Incorporates context from the encoder's output.
- **Conditional Probability & Auto-regression:** Generates each word based on the encoder's output and previously generated words.

## Instructions

1. Open the Jupyter Notebook `Transformer_Assignment_Devesh.ipynb` to view and run the code.
2. Review the PowerPoint presentation `Transformer_Presentation.pptx` for a summary of the assignment.

## Additional Resources

- [Attention is All You Need Paper](https://arxiv.org/abs/1706.03762)
- [Transformers Documentation](https://huggingface.co/transformers/)
- [Introduction to Transformer Models](https://jalammar.github.io/illustrated-transformer/)

