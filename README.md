# AI Meeting Summarizer — LED & DistilBART

**Created by Ashwin Devrani | B.Tech First Year | COER University**

## 📌 Project Overview

The AI Meeting Summarizer is a Natural Language Processing (NLP) project that automatically generates concise summaries from meeting transcripts using pretrained transformer models.

The project compares **LED (Longformer Encoder-Decoder)** and **DistilBART** using ROUGE evaluation metrics. It also identifies potential meeting decisions, extracts possible action items, and generates downloadable meeting reports.

## ✨ Features

- **Automatic Meeting Summarization:** Generates concise summaries from meeting transcripts.
- **Model Comparison:** Compares LED and DistilBART.
- **ROUGE Evaluation:** Evaluates generated summaries against reference summaries.
- **Decision Identification:** Identifies potential key decisions using keyword-based rules.
- **Action Item Extraction:** Extracts possible tasks, owners, and deadlines using rule-based techniques.
- **Interactive Web Interface:** Provides an easy-to-use interface built with Gradio.
- **Downloadable Reports:** Generates text reports containing summaries, decisions, action items, and the source transcript.

## 🧠 Models Used

| Model | Purpose |
|---|---|
| LED — `pszemraj/led-base-book-summary` | Meeting summarization |
| DistilBART — `sshleifer/distilbart-cnn-12-6` | Meeting summarization and comparison |

## 📊 Evaluation

The models are evaluated using ROUGE metrics on the test portion of the AMI Meeting Corpus.

- **ROUGE-1:** Measures unigram overlap.
- **ROUGE-2:** Measures bigram overlap.
- **ROUGE-L:** Measures the longest common subsequence overlap.

The notebook evaluates both models across 20 test meetings and compares their average ROUGE scores.

*Refer to the notebook's final evaluation output for the actual scores.*

## 🛠️ Technologies Used

- Python
- Google Colab
- Hugging Face Transformers
