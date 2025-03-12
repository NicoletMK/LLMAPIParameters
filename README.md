# Exploring LLM API Parameters in Python

This repository contains a Python script to interact with OpenAI's GPT API and experiment with different parameters that influence the model's responses. The project explores key concepts such as **temperature**, **top-p sampling**, **frequency and presence penalties**, **max tokens**, and more.

---

## Table of Contents
1. [Overview](#overview)
2. [Key Concepts](#key-concepts)
3. [Setup](#setup)
4. [Usage](#usage)
5. [Results](#results)

---

## Overview
This project demonstrates how to use the OpenAI API to generate text responses while experimenting with various parameters that control the behavior of the language model. The goal is to understand how these parameters affect the model's output and to optimize their usage for different applications.

---

## Key Concepts
The following parameters are explored in this project:
- **Temperature**: Controls the randomness of the output.
- **Top-p Sampling**: Limits the model's vocabulary to the smallest set of tokens whose cumulative probability exceeds `p`.
- **Frequency Penalty**: Discourages the model from repeating the same tokens.
- **Presence Penalty**: Encourages the model to introduce new topics or concepts.
- **Max Tokens**: Limits the length of the generated response.

---

## Setup
To set up and run this project, follow these steps:

### 1. Install Dependencies
Ensure you have Python 3.9 or later installed. Then, install the required packages:

```bash
pip install openai python-dotenv jupyter
```

### 2. Set Up OpenAI API Key

Sign up for an API key at OpenAI.\
Create a .env file in the root directory of the project and add your API key:

```bash
OPENAI_API_KEY=your-api-key-here
```
Replace your-api-key-here with your actual OpenAI API key.

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```
Then, open the explore_llm_parameters.ipynb notebook from the Jupyter interface.
To run the script, use the following command:

## Usage
The Jupyter Notebook is divided into sections that demonstrate how to:

Initialize the OpenAI client.\
Define a set of prompts.\
Generate responses using different parameter combinations.\
Analyze the results.\

## Results

The script outputs the generated responses for each parameter combination. Here’s an example of the output:
```bash
--- Default ---
Quantum computing is a technology that utilizes the principles of quantum mechanics to perform operations on data and solve problems at a much faster and more efficient rate than traditional computers.


--- Low Temperature (0.2) ---
Quantum computing is a type of computing that uses quantum bits (qubits) to perform calculations and solve problems much faster than traditional computers.


--- High Temperature (1.5) ---
Quantum computing is a form of computing that relies on the principles of quantum physics to perform calculations faster and more efficiently than traditional computers.


--- Top-p (0.9) ---
Quantum computing is the use of quantum-mechanical phenomena, such as superposition and entanglement, to perform computations more efficiently than traditional computers.


--- Frequency Penalty (1.0) ---
Quantum computing is a method of processing information using quantum bits (qubits) that can represent multiple states simultaneously and potentially perform certain calculations faster than traditional computers.


--- Presence Penalty (1.0) ---
Quantum computing is a form of computation that utilizes the principles of quantum mechanics, such as superposition and entanglement, to perform calculations faster and with greater efficiency than classical computers.


--- Max Tokens (20) ---
Quantum computing is a method of computation that uses quantum bits (qubits) and the principles
