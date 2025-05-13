# Quantifying Cognitive Bias in LLMs

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

## Project Overview
This repository is a fork and extension of the [Quantifying-Cognitive-Bias-in-LLMs](https://github.com/vsatyamuralikrishna/Quantifying-Cognitive-Bias-in-LLMs) project. It implements a simulation framework to analyze and quantify cognitive biases in Large Language Models (LLMs).

The project combines traditional trust games with the complex social dynamics of Mafia, where AI agents represent different roles and demographics. Through this framework, we analyze:
- Trust dynamics between different demographic groups
- Decision-making patterns in high-stakes situations
- The influence of role and demographic information on agent behavior
- Bias manifestation in cooperative versus competitive scenarios

## Repository Structure

```
├── Quantifying-Cognitive-bias-in-LLMs/  # Submodule containing the original project
│   ├── analysis/                        # Analysis code and data
│   ├── notebooks/                       # Jupyter notebooks
│   ├── prompts/                         # LLM prompt templates
│   └── qcbai/                          # Main package code
│
├── analysis/                           # Analysis directory
│   ├── data/                          # Data directory
│   │   └── all_results.json           # Results data
│   └── logs/                          # Experiment logs
│
├── notebooks/                         # Jupyter notebooks
```

## Setup and Installation

1. Clone the repository with submodules:
```bash
git clone --recursive https://github.com/INFO-698-InfoSci-Capstone/quant-cognitive-bias-llm.git
cd quant-cognitive-bias-llm
```

If you've already cloned the repository without submodules, you can initialize them with:
```bash
git submodule update --init --recursive
```

## Research Goals
1. Quantify demographic-based trust biases in LLM decision-making
2. Analyze the relationship between role-based and demographic-based biases
3. Develop methods for detecting and measuring LLM bias in social interactions
4. Contribute to the broader understanding of bias in AI systems

## Expected Outcomes
- Empirical data on LLM bias in trust-based decisions
- New methodologies for bias detection in social AI systems
- Contributions to the development of more equitable AI systems
- Advanced understanding of LLM behavior in complex social scenarios

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the GPL-3.0 License - see the LICENSE file for details.

## Acknowledgments
- Based on the original work from [Quantifying-Cognitive-Bias-in-LLMs](https://github.com/vsatyamuralikrishna/Quantifying-Cognitive-Bias-in-LLMs)
- Special thanks to all contributors and researchers in the field of AI bias detection

## Overview
This repository is organized as a reproducible research compendium.

## File Organization

    analysis/
    |
    ├── logs/
    │   └── log.md          # log of any progress or relevant information
    |
    ├── data/
    |   ├── all_results.json       # data obtained form scripts ran on hpc by multiple llm models
    | 
    ├── notebooks/           # analysis or results obtained from llm models
    

        

