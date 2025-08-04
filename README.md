# Synthetic Data Generator with Llama 3.2 and Unsloth

Generate high-quality synthetic question-answer datasets for LLM finetuning, using Llama 3.2, Unsloth, and Meta's synthetic-data-kit.

## Overview
This project demonstrates a full pipeline for generating synthetic Q&A data from documents (e.g., research papers), cleaning and formatting the data, and finetuning a Llama 3.2 3B model using Unsloth. The workflow is fully local and leverages state-of-the-art open-source tools for efficient data generation and model training.

## Features
- **Document ingestion**: Parse and chunk PDFs, HTML, CSV, and more
- **Synthetic Q&A generation**: Use Llama 3.2 and synthetic-data-kit to create question-answer pairs
- **Data cleaning and formatting**: Prune low-quality examples, convert to finetuning-ready formats
- **Model finetuning**: Efficient LoRA-based finetuning with Unsloth and Huggingface TRL
- **Inference and evaluation**: Run and test the finetuned model
- **Local and online model saving**: Save adapters locally or push to Huggingface Hub

## Installation
Clone the repository:
   ```bash
   git clone https://github.com/samz905/synthetic-data-generator.git
   cd synthetic_data_generator
   ```

## Usage
Open the main notebook:
```bash
jupyter notebook Synthetic_Data_Llama3_2.ipynb
```
Follow the cells step by step. The workflow includes:
- Installing dependencies
- Loading Llama 3.2 3B with Unsloth
- Ingesting a research paper (e.g., [Byte Latent Transformer: Patches Scale Better Than Tokens](https://arxiv.org/abs/2412.09871))
- Generating and cleaning Q&A pairs
- Formatting data for finetuning
- Finetuning the model with Huggingface TRL
- Running inference and saving/loading adapters

## Acknowledgements
- [Unsloth](https://github.com/unslothai/unsloth) for fast Llama finetuning
- [Meta Llama synthetic-data-kit](https://github.com/meta-llama/synthetic-data-kit) for Q&A generation
- [Huggingface TRL](https://github.com/huggingface/trl) for training utilities

## License
MIT License
