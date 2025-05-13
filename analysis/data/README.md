# README for data used in Quantifying Cognitive Bias in LLMs

## Overview 
This directory contains the data files used for analyzing cognitive biases in Large Language Models (LLMs) through our simulation framework.

## Purpose of the study 
To analyze and quantify cognitive biases in LLMs through a simulation framework, focusing on:
- Trust dynamics between different demographic groups
- Decision-making patterns in high-stakes situations
- The influence of role and demographic information on agent behavior
- Bias manifestation in cooperative versus competitive scenarios

## Structure of the data

### Model-specific Results
Each model's results are stored in separate JSON files in the notebooks directory:
- `notebooks/llama_results.json`: Results from LLaMA model simulations
- `notebooks/qwen_results.json`: Results from Qwen model simulations
- `notebooks/gemma_results.json`: Results from Gemma model simulations
- `notebooks/phi_results.json`: Results from Phi model simulations
- `notebooks/mistral_results.json`: Results from Mistral model simulations
- `notebooks/bias_scores.json`: Aggregated bias scores across all models

### all_results.json
This file contains the aggregated results from all LLM model simulations.

#### Data Format
- JSON format containing simulation results
- Includes responses and decisions from different LLM models
- Contains demographic and role-based interaction data

#### Key Components
- Model responses
- Decision patterns
- Demographic information
- Role assignments
- Interaction outcomes

#### JSON Structure
```json
{
    "model_name": "string",
    "simulation_id": "string",
    "timestamp": "string",
    "demographic_info": {
        "role": "string",
        "demographic": "string"
    },
    "interactions": [
        {
            "round": "integer",
            "decision": "string",
            "confidence": "float",
            "reasoning": "string"
        }
    ],
    "bias_metrics": {
        "trust_score": "float",
        "decision_bias": "float",
        "demographic_bias": "float"
    }
}
```

## Data Collection
The data was collected through SLURM batch jobs running multiple LLM models:
- LLaMA model simulations
- Qwen model simulations
- Gemma model simulations
- Phi model simulations
- Mistral model simulations

Each model was run through SLURM batch jobs to ensure efficient and parallel processing of the simulations.

## Data Usage
This data is used for:
- Analyzing cognitive biases in LLMs
- Quantifying bias patterns
- Understanding decision-making processes
- Evaluating trust dynamics
- Comparing bias patterns across different LLM models

## Note
Please do not edit any files in this directory manually. All data processing should be done through the appropriate scripts and notebooks.


