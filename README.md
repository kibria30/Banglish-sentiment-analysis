# Banglish Sentiment Analysis

A sentiment analysis project for Banglish text (mixture of Bengali and English) using large language models.

## Overview

This project implements sentiment classification for Banglish text using two different approaches with state-of-the-art language models.

## Implementation Files

### 1. `banglish-sentiment-ollama.ipynb`
- **Model**: Qwen2.5:14B
- **Framework**: Ollama
- **Features**:
  - Model parallelization across 2 T4 GPUs
  - Regular expression-based sentiment extraction from LLM responses
  - Supports Bengali, English, and Banglish text analysis

### 2. `banglish-sentiment-vllm.ipynb`
- **Model**: Gemma-3:4B-IT
- **Framework**: vLLM
- **Features**:
  - Optimized for faster inference and maximum GPU utilization
  - Efficient batch processing
  - High-performance text generation

## Sentiment Categories

Both implementations classify text into three categories:
- **Positive**
- **Negative** 
- **Neutral**

## Usage

1. Choose the appropriate notebook based on your requirements:
   - Use Ollama version for larger model with distributed GPU setup
   - Use vLLM version for faster inference and better resource utilization

2. Run the selected notebook to perform sentiment analysis on your Banglish dataset

## Output

The models generate predictions in a structured format with sentiment categories extracted using regular expressions, saving results to `submission.csv`.
