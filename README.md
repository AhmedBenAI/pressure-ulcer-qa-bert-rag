# Pressure Ulcer Question Answering Using BERT and Retrieval-Augmented Generation (Coursework Project)

This repository contains the code and accompanying academic paper for a coursework project exploring transformer-based question answering models for pressure ulcer management. The work evaluates two approaches:

1. Fine-tuned BERT for extractive QA
2. Retrieval-Augmented Generation (RAG) for generative QA with external knowledge retrieval

The project investigates how modern LLM-based techniques can support healthcare education by providing accurate, context-aware responses about pressure ulcer management.

## Contents
- main.ipynb  
  Jupyter notebook containing all experimentation code for dataset loading, preprocessing, BERT fine-tuning, RAG inference, and evaluation.

- Pressure-Ulcer-QA-Paper.pdf  
  Final coursework paper describing the background, methodology, dataset construction, and model comparison.

## Project Overview
This project explores whether transformer-based QA systems can support medical education by answering domain-specific questions about pressure ulcers. It compares extractive and generative QA approaches.

### Models
**BERT (extractive QA)**  
Fine-tuned on a synthetic SQuAD-style dataset (~1000 QA pairs) generated using AI from PubMed abstracts.

**RAG (generative QA)**  
Used in inference-only mode. Retrieves relevant medical text and generates a contextual answer.

## Dataset
- SQuAD format  
- Approximately 1000 QA pairs  
- Generated from PubMed abstracts  
- Not included because it is no longer available  
- Notebook code demonstrates the full training and inference pipeline

## Code Demonstrations
- Dataset preparation  
- BERT fine-tuning using HuggingFace Trainer  
- RAG inference (no fine-tuning)  
- Evaluation with BERTScore, BLEU, and F1  

## Usage
Install dependencies:
```
pip install transformers datasets evaluate torch
```

Open and run:
```
main.ipynb
```

## Paper
The included coursework paper provides complete methodology, background, and analysis.

## Notes
- Published as coursework  
- Dataset unavailable but methodology remains transparent  
- Demonstrates understanding of extractive QA, generative QA, retrieval, and evaluation
