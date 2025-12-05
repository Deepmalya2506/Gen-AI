# Gen-AI — Learn LangChain by Building Modular Generative AI Agents

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Python 3.8+](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/)

GitHub Copilot Chat Assistant

Overview

Gen-AI is a hands-on Jupyter notebook collection created to teach LangChain and practical GenAI patterns to beginners. The notebooks are designed to be modular: each section explains a concept, shows working examples, and provides exercises so you can learn by doing. This repository is your launchpad — where logic meets storytelling and every chain is a step toward clarity and creative problem solving.

Who this is for

- Beginners learning LangChain, agents, chains, and memory patterns
- Developers who prefer learning through annotated notebooks and runnable examples
- Educators who want a compact, step-by-step teaching resource

What's in this repo

- Basics.ipynb — A beginner-focused, step-by-step notebook covering fundamental LangChain concepts, building blocks (chains, agents, prompts, memory), and runnable examples.
- dataset01/ — Example dataset directory used by notebook exercises.
- images/ — Supporting images and diagrams referenced in the notebooks.
- docx.text — Example text content used in the demo.

Quickstart (Local only)

1) Prerequisites

- Python 3.8 or newer
- Git
- A terminal / command prompt and a browser

2) Clone the repo

    git clone https://github.com/Deepmalya2506/Gen-AI.git
    cd Gen-AI

3) Create and activate a virtual environment

    python -m venv .venv
    source .venv/bin/activate   # macOS / Linux
    .\.venv\Scripts\activate  # Windows (PowerShell)

4) Install recommended Python packages

The notebooks were created to be lightweight and provider-agnostic. Install the basics to run and experiment: 

    pip install --upgrade pip
    pip install jupyterlab langchain python-dotenv requests

Note: If you plan to use a specific provider SDK (for example GROQ or OpenAI), install the provider client according to their docs (see "Configuring LLM provider" below).

5) Start JupyterLab or Jupyter Notebook

    jupyter lab

Then open Basics.ipynb from the browser UI. Run cells top-to-bottom to follow the guided lessons.

Configuring LLM provider (GROQ)

This notebook was developed using GROQ as the default provider environment. Provider tooling / SDKs change over time; consult the provider docs for the latest install and authentication steps. Typical steps:

- Create a free account with your LLM / compute provider (if required).
- Set environment variables before launching the notebook. Example (bash):

    export GROQ_API_KEY="your_groq_api_key"
    export GROQ_API_BASE="https://api.groq.example"  # if applicable

If you prefer another provider (OpenAI, Hugging Face, local models), set the corresponding API key environment variables (e.g., OPENAI_API_KEY) and install the provider client. The notebook contains notes on swapping providers at the top of each example cell.

How the notebook is organized (recommended learning path)

1. Read the explanatory text cells to get conceptual context.
2. Execute the small example cells that demonstrate each concept.
3. Try the exercises at the end of each section — they are designed to be incremental.
4. Use the dataset01 files to experiment with retrieval and memory patterns.

Best practices and tips

- Run cells one-by-one the first time to understand variable changes and side effects.
- Keep your API keys out of the notebook. Use a .env file plus python-dotenv, or set environment variables in your shell.
- If a provider call fails, check rate limits and key validity before changing code.
- Use a dedicated virtual environment per project to avoid dependency conflicts.

Suggested minimal requirements file (optional)

If you want a reproducible environment, create a requirements.txt with these lines:

    jupyterlab
    langchain
    python-dotenv
    requests

License

This repository is licensed under the MIT License — a permissive, free license suitable for educational projects.

Contributing

Contributions are welcome! If you'd like to improve the notebooks (clarity, more exercises, bug fixes):

1. Fork the repository
2. Create a branch for your feature or fix
3. Commit clear, small changes and include an explanation in the notebook where appropriate
4. Open a pull request describing the change and the motivation

If you want me to apply a smaller or differently-styled README, or to produce a requirements.txt and commit it for you, tell me and I will update the repo.

Acknowledgements & resources

- LangChain documentation: https://python.langchain.com/
- Provider docs: check your provider’s official docs for authentication and SDK installation (GROQ, OpenAI, Hugging Face, etc.)

Contact

If you want changes to the README or a different license, confirm and I will update it. Enjoy learning — build small, test often, and iterate!