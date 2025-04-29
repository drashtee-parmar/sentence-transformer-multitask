# ML Apprentice Take-Home Assessment

This repository contains the implementation for a multi-task learning model using a sentence transformer. It performs topic classification (AG News) and sentiment analysis (SST-2).

## Project Structure

- `mtl_model_finetuning.ipynb`: Complete model, training loop, and inference logic
- `requirements.txt`: Python dependencies
- `Dockerfile`: Container setup for reproducibility
- `README.md`: Project overview and instructions
- `ML_Apprentice_Structured_Documentation.pdf` - Explanation and analysis

## Architectural Diagram
[mtl_architecture_diagram](mtl_architecture_diagram.jpeg)

## Setup Instructions

### 1. Install Requirements
```bash
pip install -r requirements.txt
```

### 2. Run the Notebook
Use Jupyter to open and run `mtl_model_finetuning.ipynb`.

### 3. Docker Usage
```bash
docker build -t mtl-nlp .
```

## Model Highlights

- Transformer Backbone: `sentence-transformers/all-MiniLM-L6-v2`
- Two task-specific heads (topic, sentiment)
- Supports training and evaluation across multiple tasks

## Sample Inference
Run `predict_sentences()` in the notebook to see real predictions.

