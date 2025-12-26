# Multi-label Classification of Children Stories

Multi-label text classification project on a large dataset of children stories.  
Each story is associated with **6 independent binary labels**.

Two approaches are compared:
- a **CNN trained from scratch**
- a **fine-tuned RoBERTa-base model**

---

## Task

- **Problem**: multi-label binary classification (6 labels)
- **Input**: raw text (children stories)
- **Output**: vector of 6 binary predictions
- **Main challenges**: class imbalance and threshold optimization

---

## Models

- **CNN**: custom architecture trained from scratch
- **RoBERTa-base**: pre-trained transformer fine-tuned on the dataset

---

## Training & Evaluation

- Multi-label loss functions
- Standard classification metrics (e.g. F1-score)
- Custom decision thresholds to improve weaker labels

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

