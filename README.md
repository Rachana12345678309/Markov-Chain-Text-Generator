# Text Generation using Markov Chains

This project explores the fundamentals of Markov Chains, a stochastic model describing a sequence of possible events in which the probability of each event depends only on the state attained in the previous event. It features a text generation engine that can mimic the style of various input corpora, from classic literature to modern news headlines.

## Overview

A Markov Chain is a mathematical system that experiences transitions from one state to another according to certain probabilistic rules. The defining characteristic is the **Memoryless Property**: the future depends only on the present state, not on the sequence of events that preceded it.

## Key Concepts

- **States:** The possible conditions or outcomes (e.g., individual words in a sentence).
- **Transition Probabilities:** The likelihood of moving from one state to another.
- **Transition Matrix:** A mathematical representation showing the probabilities of all possible state transitions.


## Project Objectives

- Understand the logic of **stochastic processes** and the memoryless property.
- Implement text models using the `markovify` library to generate readable, yet unpredictable sentences.
- Explore **Model Weighting**: Combining multiple text models (e.g., news headlines + Sherlock Holmes) with different weights to create unique linguistic blends.
- Identify the limitations of Markov Chains, such as short-term memory and data sparsity.

## Methods and Analysis

The project follows a specific natural language generation pipeline:

1. **Corpus Preparation:** Loading and cleaning text data (e.g., `sherlock.txt` or news headline datasets).
2. **Model Training:** Building transition matrices where the "state" is a word and the "transition" is the next word in the sequence.
3. **Sentence Synthesis:**
   - Using `make_sentence()` to generate novel text based on the learned probabilities.
   - Example output: *"medical files dropped on busy canberra road"* (a blend of news data).
4. **Ensemble Models:** Combining distinct models using `markovify.combine()` to mix styles.


## Tech Stack

- **Language:** Python 3
- **Key Library:** `markovify` (A simple, extensible Markov chain generator)
- **Environment:** Jupyter / Google Colab

## How to Run

1. **Clone this repository:**
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/markov-chain-text-gen.git
   cd markov-chain-text-gen

2. *Install dependencies:*
   pip install markovify

3. *Open the notebook:*
   jupyter notebook 33_MarkovChain.ipynb
