# Exploring LLM API Parameters in Python

This repository contains a Python script to interact with OpenAI's GPT API and experiment with different parameters that influence the model's responses. The project explores key concepts such as **temperature**, **top-p sampling**, **frequency and presence penalties**, **max tokens**, and more.

---

## Table of Contents
1. [Overview](#overview)
2. [Key Concepts](#key-concepts)
3. [Setup](#setup)
4. [Usage](#usage)
5. [Parameters](#parameters)
6. [Results](#results)
7. [Contributing](#contributing)
8. [License](#license)

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
pip install openai python-dotenv


### 2. Set Up OpenAI API Key

Sign up for an API key at OpenAI.\
Create a .env file in the root directory of the project and add your API key:
```bash
OPENAI_API_KEY=your-api-key-here
Replace your-api-key-here with your actual OpenAI API key.
Usage

To run the script, use the following command:

```bash
python explore_llm_parameters.py
Script Overview

The script performs the following tasks:

Initializes the OpenAI client.\
Defines a set of prompts.\
Generates responses using different parameter combinations.\
Prints the results for analysis.

## Results

The script outputs the generated responses for each parameter combination. Here’s an example of the output:
```bash
--- Default ---
Quantum computing is a type of computing that uses quantum bits, or qubits, which can exist in multiple states at once. This allows quantum computers to perform many calculations simultaneously, making them much faster than traditional computers for certain tasks.

--- Low Temperature (0.2) ---
Quantum computing is a type of computing that uses quantum bits, or qubits, which can exist in multiple states at once. This allows quantum computers to perform many calculations simultaneously, making them much faster than traditional computers for certain tasks.

--- High Temperature (1.5) ---
Quantum computing is like a supercharged version of regular computing. Instead of using regular bits that are either 0 or 1, it uses qubits that can be both 0 and 1 at the same time. This makes quantum computers incredibly powerful for solving complex problems.
