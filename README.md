This repository contains a BERT-to-BERT model for abstractive summarization using the CNN/DailyMail dataset. The model is based on Hugging Face's transformers library, and the code demonstrates how to preprocess, train, and evaluate a BERT encoder-decoder architecture for generating summaries from news articles.

Overview
The goal of this project is to fine-tune a BERT-to-BERT model on the CNN/DailyMail dataset for abstractive text summarization. The model is trained to generate concise summaries from long-form news articles, leveraging the encoder-decoder architecture available in the transformers library.

Features
Dataset: CNN/DailyMail dataset (version 3.0.0) containing articles and human-written highlights.

Model: Encoder-decoder architecture using BERT (bert-base-uncased) as both the encoder and decoder.

Evaluation: Model performance is evaluated using the ROUGE metric.

Training: Training is handled using Hugging Face’s Seq2SeqTrainer with custom training arguments.

Checkpointing: Model supports checkpointing to resume training in case of interruptions.

Results
Model performance is evaluated on the test set using the ROUGE metric. Some example results include:

ROUGE-1: Measures unigram overlap between the generated and reference summaries.

ROUGE-2: Measures bigram overlap.

ROUGE-L: Measures the longest common subsequence overlap.
