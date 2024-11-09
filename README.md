# Attention
Given the sentence with a masked word in the sequence, AI try to give it's best guess of what the mask word is.

## Objective
Write an AI that can predict a masked word in the sequence

### Example:
$ python mask.py
Text: We turned down a narrow lane and passed through a small [MASK].
We turned down a narrow lane and passed through a small field.
We turned down a narrow lane and passed through a small clearing.
We turned down a narrow lane and passed through a small park.

$ python mask.py
Text: Then I picked up a [MASK] from the table.
Then I picked up a book from the table.
Then I picked up a bottle from the table.
Then I picked up a plate from the table.

AI-versus-Nim
Playing Nim Game against AI


## Overview

BERT is a transformer-based language model developed by Google, trained to predict masked words within a text sequence by considering the surrounding context. This project involves two parts:
1. **Predicting Masked Words**: Using the Hugging Face `transformers` Python library to load the BERT model and predict masked words in sentences.
2. **Visualizing Attention**: Generating diagrams that display attention scores across BERT’s 144 self-attention heads to analyze which words the model focuses on in each layer.

## Solution
The code uses a BERT model to predict missing words in a sentence. It breaks the sentence into pieces, feeds it to the model, and the model predicts the missing word. Finally, it shows how the model focused on different parts of the sentence to make its prediction.

## Usage:
Requires Python(3) and Python package installer pip(3) to run:

Install requirements: $pip3 install -r requirements.txt

Run Game: $python mask.py
