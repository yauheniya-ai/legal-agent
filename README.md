# AI Legal Agent: Big Tech Tax Analysis

An intelligent agent that analyzes 10-K company filings to examine the potential effects of Pillar Two OECD reform on major tech companies using LangChain, LangGraph, Google Gemini, and FAISS.

## 📊 Analysis Results

<div style="text-align: center;">

  <img src="./data/output/tax_etr_2024.png" alt="Tax and ETR in 2024" width="800" />

  <p style="color:gray; font-style: italic; margin-top: 0.5em;">
    Matplotlib for Charting & ChatGPT for Generating the Background Image
  </p>

</div>


## 🚀 Quick Start

### Prerequisites
- Python 3.12+
- Google Gemini API key

### Installation
```bash
# Clone the repository
git clone https://github.com/yauheniya-ai/legal-agent
cd legal-agent

# Create virtual environment (recommended: use uv for speed)
uv venv --python=3.12
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies
uv pip install -r requirements.txt
```

### Usage
1. Rename `.env.example` to `.env` and set your Google Gemini API key 
2. Open `legal-agent.ipynb` in your IDE or in Jupyter
3. Run all cells to process the 10-K documents and generate analysis

## 📁 Project Structure

```
├── assets/                 # Company logos and visualizations
├── data/
│   ├── input/             # 10-K PDF documents (2024 filings)
│   └── output/            # Generated Excel reports and charts
├── faiss_index/           # Vector database for document embeddings
├── legal-agent.ipynb      # Main analysis notebook
└── requirements.txt       # Python dependencies
```

## 🔧 Key Technologies

- **LangChain**: Orchestration framework
- **LangGraph**: Workflow management
- **Google Gemini**: Language model (2.0-flash & 2.5-pro-preview)
- **FAISS**: Vector similarity search
- **PyPDF**: PDF document processing
- **Pydantic**: Structured data extraction

## 📈 Features

- **Document Processing**: Handles 99-168 page 10-K filings
- **Intelligent Retrieval**: Company-specific information extraction
- **Memory-Powered Reports**: Generates comprehensive analysis with citations
- **Structured Data Extraction**: Precise financial metrics extraction
- **Visualization**: Tax burden and ETR analysis chart

## 🎯 Use Cases

- Tax strategy analysis for multinational corporations
- OECD Pillar Two compliance assessment
- Financial document intelligence
- Legal research automation

## 📚 Tutorial Series

This project is part of a three-part tutorial series:
- **Part 1**: [Introduction to LangChain and classification/extraction](https://github.com/yauheniya-ai/langchain-intro)
- **Part 2**: [Implementing RAG (Retrieval-Augmented Generation)](https://github.com/yauheniya-ai/langchain-rag)
- **Part 3**: Building the complete AI Legal Agent (this project)

## ⚖️ Pillar Two OECD Reform

The Pillar Two reform establishes a global minimum tax of 15% for multinational enterprises. This agent analyzes how major tech companies might be affected by these new regulations.

## 📄 License

The MIT License permits free use, modification, and distribution of software with attribution.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📚 Further Information

There is a detailed [article on Medium](https://medium.com/@yauheniya.ai/building-an-ai-legal-agent-how-to-analyze-big-techs-tax-strategies-in-minutes-not-hours-1791dec1cfba) explaining the implementation steps.
