# Building-a-RAG-System-with-Ollama-smollm2-
# Financial Document Analysis RAG System

An intelligent document analysis system that combines Retrieval Augmented Generation (RAG) with Large Language Models(smollm2) to perform sophisticated financial analysis.

## 🚀 Features

- **Multi-perspective Analysis:**
  - Financial Metrics Analysis
  - Risk Assessment
  - Market Analysis
- **Specialized Prompts:** Custom-designed prompts for each analysis type
- **Document Processing:** Efficient PDF processing and chunking
- **Advanced Retrieval:** Semantic search using HuggingFace embeddings
- **Structured Output:** Professional-grade financial insights

## 🛠️ Technical Stack

- **LangChain:** For document processing and RAG implementation
- **smollm2:** Base language model
- **HuggingFace Embeddings:** all-MiniLM-L6-v2 model
- **ChromaDB:** Vector store for efficient retrieval
- **PyPDF:** PDF document processing

## 📋 Prerequisites

```bash
pip install langchain chromadb sentence_transformers pypdf ollama
```

## 🚀 Quick Start

1. **Install Ollama:**
```bash
curl https://ollama.ai/install.sh | sh
ollama serve
ollama pull smollm2
```

2. **Initialize the System:**
```python
from finance_rag import FinanceRAG

# Process your document
rag = FinanceRAG()
components = process_financial_document("your_document.pdf")
```

3. **Perform Analysis:**
```python
# Financial Analysis
financial_analysis = analyze_document(components, 
    "What are the key financial metrics?", 'financial')

# Risk Assessment
risk_analysis = analyze_document(components,
    "What are the main risk factors?", 'risk')

# Market Analysis
market_analysis = analyze_document(components,
    "What are the market opportunities?", 'market')
```

## 💡 Key Components

### FinanceRAG Class
The main class that handles:
- Document loading and processing
- Text splitting and embedding
- Vector store setup
- Specialized analysis chains

### Analysis Types

1. **Financial Analysis**
   - Focus on quantitative data
   - Key financial metrics
   - Trend analysis
   - Data-driven insights

2. **Risk Assessment**
   - Market risk
   - Credit risk
   - Operational risk
   - Liquidity risk
   - Regulatory risk

3. **Market Analysis**
   - Market trends
   - Competitive analysis
   - Growth opportunities
   - Industry benchmarks

## 📊 Example Output Structure

Each analysis type provides structured output:

### Financial Analysis
1. Key Financial Metrics
2. Trend Analysis
3. Risk Assessment
4. Recommendations

### Risk Assessment
1. Risk Identification
2. Risk Quantification
3. Mitigation Strategies
4. Overall Risk Rating

### Market Analysis
1. Market Overview
2. Competitive Position
3. Growth Analysis
4. Strategic Recommendations

## 🤝 Contributing

Feel free to:
- Fork the repository
- Create a feature branch
- Submit pull requests
- Report issues
## 🙏 Acknowledgments

- LangChain community
- Ollama team
- HuggingFace team
- All contributors and users

---
