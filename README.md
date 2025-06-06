# AI Legal Agent: Big Tech Tax Analysis

An intelligent agent that analyzes 10-K company filings to examine the potential effects of Pillar Two OECD reform on major tech companies using LangChain, LangGraph, Google Gemini, and FAISS.

## 📊 Analysis Results

| Company   | ETR 2024 (%) | US Tax 2024 ($M) | Foreign Tax 2024 ($M) |
|-----------|--------------|-------------------|----------------------|
| Alphabet  | 16.4         | 22,485           | 2,468               |
| Microsoft | 18.2         | 14,531           | 9,858               |
| NVIDIA    | 12.0         | 6,045            | 502                 |

## 🚀 Quick Start

### Prerequisites
- Python 3.12+
- Google Gemini API key

### Installation
```bash
# Clone the repository
git clone <repository-url>
cd ai-legal-agent

# Create virtual environment (recommended: use uv for speed)
uv venv --python=3.12
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies
uv pip install -r requirements.txt
# or: pip install -r requirements.txt
```

### Usage
1. Set your Google Gemini API key as an environment variable
2. Open `legal-agent.ipynb` in Jupyter
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
- **LangGraph**: Complex workflow management
- **Google Gemini**: Language model (2.0-flash & 2.5-pro-preview)
- **FAISS**: Vector similarity search
- **PyPDF**: PDF document processing
- **Pydantic**: Structured data extraction

## 📈 Features

- **Document Processing**: Handles 99-168 page 10-K filings
- **Intelligent Retrieval**: Company-specific information extraction
- **Memory-Powered Reports**: Generates comprehensive analysis with citations
- **Structured Data Extraction**: Precise financial metrics extraction
- **Visualization**: Tax burden and ETR analysis charts

## 🎯 Use Cases

- Tax strategy analysis for multinational corporations
- OECD Pillar Two compliance assessment
- Financial document intelligence
- Legal research automation

## 📚 Tutorial Series

This project is part of a three-part tutorial series:
- **Part 1**: Introduction to LangChain and classification/extraction
- **Part 2**: Implementing RAG (Retrieval-Augmented Generation)
- **Part 3**: Building the complete AI Legal Agent (this project)

## ⚖️ Pillar Two OECD Reform

The Pillar Two reform establishes a global minimum tax of 15% for multinational enterprises. This agent analyzes how major tech companies might be affected by these new regulations.

## 📄 License

[Include your license information here]

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

**Happy agent development!** 🤖⚖️