# LLM Engineering Workspace

A comprehensive learning and experimentation repository covering various aspects of Large Language Model (LLM) engineering, from fundamentals to advanced implementations.

## 📁 Workspace Structure

### 1. LLM Engineering Basics
**Path:** `01-llm-engineering-basics/`

Foundational notebooks for getting started with LLM applications:
- **ollama-website-summarizer.ipynb** - Web scraping and summarization using local Ollama models
- **gpt-website-summarizer.ipynb** - Website content summarization using OpenAI's GPT models
- **company-details-brochure-generator.ipynb** - Generate marketing content from company information
- **code-tutor.ipynb** - Interactive code tutoring assistant

**Key Topics:** Basic LLM API interactions, prompt engineering, text summarization, content generation

---

### 2. Experiments with Frontier Models
**Path:** `02-experiments-with-frontier-models/`

Experiments and applications using cutting-edge frontier LLMs:
- **frontier-models-api-experiments.ipynb** - API exploration and testing
- **conversational-ai.ipynb** - Building conversational chatbot interfaces
- **simple-llm-interface-with-gradio.ipynb** - Creating UI with Gradio framework
- **airline-ai-assistant.ipynb** - Domain-specific assistant for airline operations
- **airline-ai-assistant-multimodal.ipynb** - Multimodal AI handling text and images

**Supporting Files:**
- `scraper.py` - Web scraping utilities
- `hamlet.txt` - Sample text data for testing

**Key Topics:** API integration, conversational design, UI frameworks, multimodal inputs

---

### 3. Experiments with Open Source Models
**Path:** `03-experiments-with-open-source-models/`

Working with open-source LLM ecosystems:
- **connecting-to-hugging-face.ipynb** - Hugging Face integration and authentication
- **understanding-hugging-face-pipelines.ipynb** - Using Hugging Face pipelines for NLP tasks

**Key Topics:** Open-source models, Hugging Face Hub, community models, local deployment

---

### 4. LLM Selection
**Path:** `04-llm-selection/`

Comparative analysis and selection of LLMs for different scenarios:
- **frontier-llm-compare-python-cpp-converter.ipynb** - Comparing frontier models with Python/C++ implementations
- **open-source-llm-compare-python-cpp-converter.ipynb** - Comparing open-source models with Python/C++ implementations
- **llm-compare-python-cpp-rust-converter.ipynb** - Multi-language comparison (Python, C++, Rust)

**Key Topics:** Model benchmarking, performance comparison, language implementation differences, cost-benefit analysis

---

### 5. Retrieval-Augmented Generation (RAG)
**Path:** `05-retrieval-augmented-generation/`

Comprehensive RAG pipeline implementations with insurance QA assistant use case:

**Core Notebooks:**
1. **insurance-qa-assistant-simplistic-brute-force-rag.ipynb** - Basic RAG without optimization
2. **insurance-qa-assistant-embeddings-with-chroma.ipynb** - Using embeddings and vector databases
3. **insurance-qa-assistant-rag-pipeline-with-ui.ipynb** - Complete pipeline with user interface
4. **insurance-qa-assistant-evaluating-rag-pipeline.ipynb** - Evaluation and metrics
5. **insurance-qa-assistant-advanced-rag-without-langchain.ipynb** - Custom RAG implementation

**Supporting Components:**
- `app.py` - Main application entry point
- `evaluator.py` - RAG pipeline evaluation metrics
- `implementation/` - Standard RAG implementation modules
- `advanced_implementation/` - Advanced custom RAG modules
- `evaluation/` - Evaluation scripts and test data
- `knowledge-base/` - Company, contracts, employees, and products documentation
- `preprocessed_db/` - Chroma vector database with cached embeddings

**Key Topics:** Vector embeddings, semantic search, Chroma DB, evaluation metrics, production RAG

---

### 6. Fine-tuning Frontier Models
**Path:** `06-fine-tuning-frontier-models/`

Fine-tuning and customization of frontier LLMs:

**Preparation & Training:**
- **dataset-preparation.ipynb** - Data collection and preprocessing
- **dataset-preprocessing.ipynb** - Advanced data cleaning and formatting
- **baseline-machine-learning-models.ipynb** - Baseline model performance
- **shallow-neural-network-and-llm.ipynb** - Neural network fundamentals
- **gpt-4.1-nano-fine-tuning.ipynb** - Fine-tuning GPT models

**Specialized Use Cases:**
- **redemption_train.ipynb** - Training for pricing/redemption scenarios
- **redemption_run.ipynb** - Running trained models
- **results.ipynb** - Results analysis and visualization

**Supporting Files:**
- `human_in.csv` / `human_out.csv` - Training data
- `jsonl/` - Fine-tuning dataset in JSONL format
- `pricer/` - Pricing model implementations

**Key Topics:** Fine-tuning workflows, dataset preparation, performance optimization, domain adaptation

---

### 7. Fine-tuning Open Source Models
**Path:** `07-fine-tuning-open-source-models/`

Fine-tuning and optimization of open-source LLMs:

**Training Pipeline:**
1. **understanding-qlora.ipynb** - QLoRA technique for efficient fine-tuning
2. **dataset-preparation.ipynb** - Preparing datasets for open-source models
3. **training.ipynb** - Training open-source models
4. **evaluation.ipynb** - Evaluating fine-tuned models
5. **results.ipynb** - Results analysis

**Supporting Files:**
- `util.py` - Utility functions for training
- `pricer/` - Domain-specific pricing models

**Key Topics:** QLoRA, parameter-efficient fine-tuning, open-source model optimization, adapter training

---

### 8. Agentic AI Introduction
**Path:** `08-agentic-ai-introduction/`

*This folder is currently empty and reserved for future agentic AI implementations.*

**Expected Topics:** Agent design patterns, tool usage, autonomous decision-making, multi-step reasoning

---

## 🛠️ Setup

### Prerequisites
- Python 3.8+
- Virtual environment (`venv` or `conda`)
- Git

### Installation

1. Clone the repository:
```bash
git clone <repo-url>
cd llm-engineering
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

Or using the project configuration:
```bash
uv sync
```

---

## 🔑 Key Technologies & Frameworks

- **LLM APIs:** OpenAI GPT, Ollama, Hugging Face
- **Vector Databases:** Chroma DB
- **UI Frameworks:** Gradio
- **Fine-tuning:** QLoRA, LoRA
- **Languages:** Python, C++, Rust
- **Utilities:** Jupyter Notebooks, pandas, numpy

---

## 📊 Project Structure

```
llm-engineering/
├── 1. llm-engineering-basics/
├── 2. experiments-with-frontier-models/
├── 3. experiments-with-open-source-models/
├── 4. llm-selection/
├── 5. retrieval-augmented-generation/
├── 6. fine-tuning-frontier-models/
├── 7. fine-tuning-open-source-models/
├── 8. agentic-ai-introduction/
├── pyproject.toml
├── README.md
└── .env
```

---

## 📝 Notes

- Each folder is self-contained and can be explored independently
- Notebooks are ordered sequentially for progressive learning
- Environment variables should be configured in `.env` for API credentials
- Vector database files are cached in `5. retrieval-augmented-generation/preprocessed_db/`

---

## 🚀 Getting Started

1. Open any notebook in VS Code
2. Select the Python kernel
3. Run cells sequentially
4. Experiment with parameters and prompts

---

## 📄 License

[Add your license information here]

---

**Last Updated:** February 2026
