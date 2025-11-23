# Transformers, what can they do?

This Jupyter notebook provides a comprehensive introduction to the capabilities of the Hugging Face Transformers library through practical examples and demonstrations.

## Overview

The notebook demonstrates various Natural Language Processing (NLP) tasks that can be performed using pre-trained transformer models through the Hugging Face Transformers library. It showcases how to use simple pipelines to accomplish complex NLP tasks with just a few lines of code.

## Prerequisites

Before running this notebook, you need to install the following libraries:

```bash
pip install datasets evaluate transformers[sentencepiece]
```

## What's Inside

The notebook covers the following NLP tasks and capabilities:

### 1. Sentiment Analysis
- Analyze the sentiment (positive/negative) of text inputs
- Process single texts or batches of texts
- Examples include simple sentences and longer book reviews

### 2. Zero-Shot Classification
- Classify text into categories without specific training on those categories
- Demonstrates classification of course descriptions and book reviews
- Shows how to use custom candidate labels for classification

### 3. Text Generation
- Generate text continuations based on input prompts
- Control generation parameters like max length and number of sequences
- Uses models like GPT-2 and DistilGPT-2

### 4. Fill-Mask (Masked Language Modeling)
- Predict missing words in sentences
- Uses masked tokens (e.g., `<mask>`) to identify words to predict
- Returns top-k predictions with confidence scores
- Note: Different models may use different mask tokens

### 5. Named Entity Recognition (NER)
- Identify and classify named entities in text
- Recognizes entities such as:
  - Persons (PER)
  - Locations (LOC)
  - Organizations (ORG)
- Groups related entities together using `grouped_entities=True`

### 6. Question Answering
- Extract answers to questions from given context
- Demonstrates contextual understanding of the model
- Returns the answer along with confidence scores

### 7. Text Summarization
- Generate concise summaries of longer texts
- Useful for condensing articles, documents, and reports
- Example includes summarizing a text about engineering education in America

### 8. Translation
- Translate text between different languages
- Examples include:
  - French to English translation
  - English to Traditional Chinese (ZH_TW)
  - Traditional Chinese back to English
- Uses various pre-trained translation models from the Helsinki-NLP and community contributors

## How to Use

1. Open the notebook in Jupyter, Google Colab, or any compatible environment
2. Run the first cell to install all required dependencies
3. Execute cells sequentially to see demonstrations of each NLP task
4. Modify the example texts to experiment with your own data
5. Customize pipeline parameters (e.g., model selection, max_length, top_k) to suit your needs

## Key Features

- **Simple API**: All tasks use the same `pipeline` interface for consistency
- **Pre-trained Models**: Leverages state-of-the-art pre-trained models without requiring training
- **Flexible**: Easy to switch between different models for the same task
- **Interactive**: Can be run step-by-step to understand each capability

## Learning Outcomes

After working through this notebook, you will understand:
- How to use the Transformers library for common NLP tasks
- The variety of tasks that transformer models can perform
- How to configure pipelines with different models and parameters
- Practical applications of NLP in real-world scenarios

## Additional Resources

- [Hugging Face Transformers Documentation](https://huggingface.co/docs/transformers/)
- [Hugging Face Course](https://huggingface.co/course)
- [Model Hub](https://huggingface.co/models)

## Note

This notebook is part of the Hugging Face NLP course and serves as an introductory guide to the capabilities of transformer models. Each section can be expanded with more examples and customization based on your specific use case.
