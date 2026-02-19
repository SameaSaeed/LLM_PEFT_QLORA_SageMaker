# LLM_PEFT_Quantization

## Introduction

LLM_PEFT_Quantization is a comprehensive repository designed to demonstrate the fine-tuning of Large Language Models (LLMs) using Parameter Efficient Fine-Tuning (PEFT) techniques and quantization. This solution provides a robust pipeline for data preparation, model configuration, training, evaluation, and deployment, specifically optimized for scalable and cost-effective workflows.

## Features

- End-to-end pipeline for PEFT-based LLM fine-tuning and Quantization
- Data preprocessing 
- Deployment approach for launching and monitoring endpoints

## Requirements

- Python 3.8 or later
- torch, transformers, datasets, and accelerate libraries
- Additional dependencies defined in `requirements.txt`

## Approach

### 1. Prepare Your Dataset

- Place your training and evaluation datasets in the `data/` directory.
- Use the provided scripts to clean and tokenize your data.

### 2. Configure Training Parameters

- Edit the configuration to set your model, data paths, hyperparameters, and settings.
- Choose options for PEFT and QLoRA in the configuration.

### 3. Launch Training 

- Start a training job:
- Monitor logs and training progress in the console.

### 4. Evaluate the Fine-Tuned Model

- After training, use the evaluation utilities to evaluate model.

### 5. Deploy the Model

- Deploy your trained model to an endpoint:
- Invoke the endpoint for real-time predictions using the client script.

## System Workflow Overview

```mermaid
flowchart TD
    A[Data Preparation] --> B[Model Configuration]
    B --> C[Launch Training]
    C --> D[Model Evaluation]
    D --> E[Model Deployment]
    E --> F[Endpoint Inference]
```
## Sample Output 

(Ollama-based-for local CPU based inferencing)

<img width="227" height="250" alt="ollama_output" src="https://github.com/user-attachments/assets/d59a63bc-796b-4ed9-8acd-62910c93c5f8" />


(vLLM for production-grade GPU based inferencing)


<img width="380" height="53" alt="vLLM_output" src="https://github.com/user-attachments/assets/4e480caf-3ac0-4856-a93c-f3e34e07b45d" />


## Support

For issues or questions, please open an issue in the repository or contact the maintainer via GitHub.

This repository is licensed under the MIT License. See the LICENSE file for details.
