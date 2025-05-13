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
This file contains the aggregated results from all LLM model simulations. Each prompt is run multiple times to ensure statistical significance.

#### Data Format
- JSON format containing simulation results
- Includes demographic information and persona details
- Contains multiple responses for each prompt
- Includes timestamps and execution details

#### Key Components
- Demographic information (gender, race, ethnicity)
- Persona details and prompt information
- Multiple responses per prompt
- Decision and reasoning for each response
- Timestamps and execution metadata

#### JSON Structure
```json
{
    "gender": "string",
    "race": "string",
    "ethnicity": "string or null",
    "persona": "string",
    "style": "string",
    "prompt_name": "string",
    "prompt_id": "string",
    "execution_id": "string",
    "date": "string",
    "time": "string",
    "timestamp": "string",
    "prompt_responses": {
        "responses": [
            {
                "id": "string",
                "response_text": "string",
                "decision": "string",
                "reason": "string",
                "response": "boolean",
                "iteration": "integer",
                "response_time": "float",
                "timestamp": "string"
            }
        ]
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

Each model was run through SLURM batch jobs to ensure efficient and parallel processing of the simulations. Each prompt is executed multiple times to gather statistically significant results.

## Data Usage
This data is used for:
- Analyzing cognitive biases in LLMs
- Quantifying bias patterns
- Understanding decision-making processes
- Evaluating trust dynamics
- Comparing bias patterns across different LLM models

## Note
Please do not edit any files in this directory manually. All data processing should be done through the appropriate scripts and notebooks.


