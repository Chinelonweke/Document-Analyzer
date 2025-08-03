# 🚀 DocTalk: AI-Powered Document Conversations

## ✨ Overview
**Chat with any PDF like it's your smartest friend** - A zero-cost document Q&A app built during *AI Summer of Code Season 2* that remembers your conversation context.

## 🌟 Features
- **Natural conversations** with your documents
- **Context-aware** (remembers previous questions)
- **100% free stack** (no hidden costs)
- **Lightning fast** (<1s responses via Groq)
- **Private processing** (local embeddings)

## 🛠️ Tech Stack
| Component       | Use Case                          |
|----------------|----------------------------------|
| ![Groq](https://img.shields.io/badge/Groq-FF6C37?style=for-the-badge) | Blazing-fast LLM inference |
| ![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21F?style=for-the-badge) | Local text embeddings |
| ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge) | Web interface |
| ![LangChain](https://img.shields.io/badge/LangChain-00A67E?style=for-the-badge) | Document processing |
| ![FAISS](https://img.shields.io/badge/FAISS-7289DA?style=for-the-badge) | Vector similarity search |

## 🏃‍♂️ Quick Start

### 1. Prerequisites
```bash
Python 3.9+
```
### 2. Installation
```bash
git clonehttps://github.com/Chinelonweke/Document-Analyzer.git
pip install -r requirements.txt
```

### 3. Configure
Create .env file:

``` env
GROQ_API_KEY=your_key_here
```

### 4. Launch
``` bash
streamlit run app.py
```

#### 🧠 How It Works
### 🔍 RAG Architecture
### 1. Document Processing

PDF → Text chunks (with overlap)

Local embeddings via all-MiniLM-L6-v2

### 2.Conversation Flow

Maintains last 5 Q&A pairs

Dynamic context injection

### 3. Response Generation

Groq's ultra-fast inference

Document-grounded answers

#### ⚙️ Configuration
### Model Options
```python
MODELS = {
    "llama-3.1-8b-instant": "Fast & Smart (131k context)",
    "llama-3.3-70b-versatile": "Most Capable (131k context)", 
    "gemma2-9b-it": "Balanced (8k context)"
}
``` 

#### Performance Tweaks
Parameter	Default	Description
chunk_size	1000	Characters per chunk
chunk_overlap	200	Context preservation
max_history	5	Conversation memory

#### 📂 Project Structure
### 1. Core Files

``` text
doc-talk/
├── app.py                # Main application        
└── requirements.txt      # Dependencies
```

### 2. Supporting Directories

``` text
├── assets/               # Sample PDFs
│   └── example.pdf
└── utils/                # Helper modules
    ├── embeddings.py
    └── conversation.py
```

#### 🚨 Troubleshooting
#### Common Issues
#### 1. "No relevant info"

Try different PDF/rephrase question

### 2. Rate limits

Wait 1min or upgrade account

### 3. Context confusion

Clear conversation history

#### 🎓 Learning Outcomes
1. RAG pattern implementation

2. Vector database usage

3. Conversation state management

4. Production deployment

####  🤝 Contributing
1. Fork the repository

2. Create your feature branch

3. Submit a PR!

#### 📜 License
MIT - Use freely for learning and building!

### Made with ❤️ during AI Summer of Code
Special thanks to:

1. Mentors

2. Open-source maintainers

3. Groq for their free tier

``` text

Key changes made:
1. Converted all bullet points to numbered lists where appropriate
2. Maintained nested numbering for hierarchical information
3. Kept tables for non-sequential information
4. Preserved all original functionality and vibe
5. Added numbering to acknowledgments section

The Markdown will now render with proper numbering throughout while keeping the engaging style. Let me know if you'd like any adjustments to the numbering format!
```
