# mini project 9: NLP Application: Content Moderation with Transformers

## Project overview
 The project builds an automated content moderation classifier for SafeSpace AI that distinguishes between hate speech, offensive language, and neutral content in social media posts. It compares a traditional TF-IDF + Logistic Regression baseline against a fine-tuned DistilBERT transformer, finding that while both models achieve ~90% overall accuracy, both struggle to detect the minority hate speech class — a critical limitation addressed through a proposed three-tier human-in-the-loop moderation workflow.

## Dataset
**Dataset title:** Twitter Hate Speech and Offensive Language Dataset
**Source:** [GitHub](https://github.com/t-davidson/hate-speech-and-offensive-language)


## Setup instructions

Run this command to install all dependancies 

```bash
pip install -r requirements.txt
```

dataset is automatically downloaded when runnning the notebook

## How to run the code

1. Clone the repository:

```bash
git clone https://github.com/bigz4/mini-project-9
```

2. Run all cells in mini_project_9.ipynb

## Experimental Results
| metric | tfidf_logistic_regression | distilbert_finetuned |
| --- | --- | --- |
| accuracy | 0.9024 | 0.9161 |
| weighted_f1 | 0.8959 | 0.9112 |
| hate_speech_f1 | 0.33 | 0.39 |
| hate_speech_recall | 0.26 | 0.32 |
| offensive_f1 | 0.94 | 0.95 |
| neither_f1 | 0.86 | 0.90 |
| macro_f1 | 0.71 | 0.74 |

## Team member contributions
 * ** Nicky Cheng ** - Jupyter notebook, Final report, ReadME, Github
 * ** Brendan Zapf ** - Jupyter notebook, Final report, ReadME, Github