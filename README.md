# Named Entity Recognition (NER) with Transformers 

This repository contains Jupyter Notebooks for fine-tuning popular Transformer-based models — **RoBERTa**, **DistilBERT**, and **BERT** — on a Named Entity Recognition (NER) task.  
It also includes a **Gradio-based web interface** to easily test the trained models interactively.

---

## Dataset
We used the **[Name Entity Recognition (NER) Dataset](https://www.kaggle.com/datasets/debasisdotcom/name-entity-recognition-ner-dataset)** from Kaggle.  
The dataset contains sentences labeled with entities like **PER** (Person), **ORG** (Organization), **LOC** (Location), **DATE**, etc.

---

## Models Used

1. BERT (bert-base-cased)
2. DistilBERT (distilbert-base-cased)
3. RoBERTa (roberta-base)

---

## Example Input & Output

**Input sentence:** Harry Potter was a student at Hogwarts


**Model output:**
```json
[
  {
    "entity": "PER",
    "score": 0.99,
    "start": 0,
    "end": 11,
    "word": "Harry Potter"
  },
  {
    "entity": "ORG",
    "score": 0.98,
    "start": 25,
    "end": 33,
    "word": "Hogwarts"
  }
]
```
### Install dependencies:
pip install -r requirements.txt

### requirements.txt should include:
```
transformers
datasets
torch
gradio
pandas
numpy
scikit-learn
```





