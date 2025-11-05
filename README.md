# Building Intelligent Financial Agents with Agno AGI

Welcome to the **Agentic Finance Bootcamp** demo project!  

This repository provides a ready-to-use Python environment using **uv** and the **Agno** framework to explore the world of AI agents.

---

## Prerequisites
Please ensure you have the following installed before starting

## 1. Install `uv` (Python package manager)
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh     # Install uv
source $HOME/.local/bin/env                         # Add uv to your shell path
uv --version                                        # Verify installation
```

## 2. Install LM Studio
LM Studio allows you to run large language models (LLMs) locally on your machine. Download and install LM Studio from the [official site](https://lmstudio.ai/download). Launch LM Studio and start the local API server from the sidebar. By default, it runs at http://localhost:1234/v1 

## 3. Load Local Models 
Download the following models directly from within LM Studio using the “Models” tab.
LM Studio automatically saves them in the correct location and format.

    •	gpt-oss-20b	 							→ for general-purpose agent reasoning with tool use

	•	text-embedding-nomic-embed-text-v1.5 	→ for embedding and retrieval tasks

Choose GGUF for non-M series Macs. LMStudio ships with a built-in lightweight embedding service (based on nomic-embed-text or equivalent) for local compatibility with OpenAI-style /v1/embeddings APIs. 

## Setup Instructions

```bash
git clone https://github.com/kannansingaravelu/agno-demo.git 
cd agno-demo                                                  
uv venv --python 3.13 .venv                         # Create venv with python 3.13
uv sync                                         	# Install dependencies                                                     
uv run examples/main.py								# Run sample demo                             
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

## System Compatibility 

**Note:**
This demo was developed and will be presented using Apple Silicon (M-series) Macs. Model formats and runtime performance are optimized for macOS + M-series chips.

If you’re using Windows, Linux, or Intel-based macOS, please:

	•	Download model variants compatible with your system.
	•	Configure LM Studio or Ollama accordingly.
	•	Expect minor differences in setup or performance.

**Bootcamp Scope:**
The bootcamp will not cover installation procedures for other operating systems. Participants using non-macOS systems are encouraged to adapt the setup steps independently or refer to their platform’s documentation.
