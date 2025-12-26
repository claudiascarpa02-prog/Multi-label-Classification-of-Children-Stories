# Multi-label Classification of Children Stories
[![Python](https://img.shields.io/badge/python-3.10-blue)](https://www.python.org/) 
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Classifying children stories into **6 categories** using **CNNs** and **transformers (RoBERTa)**.  
Each story can have multiple labels. The project addresses **class imbalance** and **threshold optimization**.

---

## Task
- **Type:** Multi-label binary classification (6 labels)  
- **Input:** Raw text (children stories)  
- **Output:** Vector of 6 binary predictions  
- **Challenges:** Class imbalance, weak-label threshold optimization

---

## Models
1. **CNN**: Custom architecture trained from scratch  
2. **RoBERTa-base**: Pre-trained transformer fine-tuned on the dataset  

### Architecture Diagram of the CNN
IMMAGINE

---

## Training & Evaluation
- Multi-label loss functions  
- Standard metrics: **F1-score**, **accuracy**  
- Custom thresholds for weaker labels  

## Results

### F1-Score by Model
| Tag           | RoBERTa | CNN    |
|---------------|---------|--------|
| BadEnding     | 0.9391  | 0.8742 |
| Conflict      | 0.5753  | 0.4271 |
| Dialogue      | 0.9396  | 0.9160 |
| Foreshadowing | 0.5687  | 0.4395 |
| MoralValue    | 0.8780  | 0.8150 |
| Twist         | 0.9154  | 0.8654 |

---

## Repository Structure


├── cnn_training.py          # Training pipeline for the CNN model  
├── roberta_training.py      # Fine-tuning procedure for RoBERTa  
├── evaluate_models.py       # Loads best saved models and evaluates them  
└── report.pdf               # Final project report  


---


## Trained Models

Due to their size, trained model checkpoints are not included in the repository.

They are publicly available at [this link](https://drive.google.com/drive/folders/1Y8tpu24vhWwJXxj8jdYRPNnrsaI-aq_f?usp=drive_link)

Download the files and place them inside a local `saved_models/` directory before running the evaluation script.

---

## Usage

### 1. Clone & install dependencies
```bash
git clone <repository-url>
cd Multi-label-Classification-of-Children-Stories
pip install -r requirements.txt
