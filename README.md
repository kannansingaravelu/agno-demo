# Agentic Finance Bootcamp by Kannan Singaravelu

Welcome to the **Agentic Finance Bootcamp** demo project!  

This repository provides a ready-to-use Python environment using **uv** and the **Agno** framework to explore the world of AI agents.

---

## Prerequisites
Please ensure you have the following installed before starting

## 1. Install `uv` (Python package manager)
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh     # install from source
source $HOME/.local/bin/env                         # set uv path
uv --version                                        # check uv installation
```

## 2. Install LM Studio
Download and install LM Studio from the official site:
> https://lmstudio.ai/download 

LM Studio allows you to run large language models (LLMs) locally on your machine.

## 3. Load Local Models 
**Best Option**: Download the following models directly from within LM Studio using the “Models” tab.
LM Studio automatically saves them in the correct location and format.

Recommended Models:

    •	gpt-oss-20b → for general-purpose agent reasoning with tool use

	•	bge-small-en-v1.5 → for embedding and retrieval tasks

Choose GGUF for non-M series Macs.


## Setup Instructions

```bash
git clone https://github.com/kannansingaravelu/agno-demo.git    # clone this repository
cd agno-demo                                                    # change directory 
uv venv --python 3.13 .venv                                     # create venv with python 3.13
uv sync                                                         # install dependencies
uv run examples/main.py                                         # run sample demo
```

## Project Structure
```bash
agno-demo/
├── pyproject.toml         
├── uv.lock                
├── README.md              
├── .gitignore             
└── examples/
    └── main.py            
```
