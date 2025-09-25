# Local AI Agent - Restaurant Review QA System

This project implements a local question-answering system for restaurant reviews using LangChain and Ollama. It uses vector embeddings to perform semantic search on restaurant reviews and generates relevant answers using a local LLM.

## Features

- Local LLM-powered question answering
- Vector-based semantic search for relevant reviews
- Persistent vector storage using Chroma DB
- Interactive command-line interface

## Prerequisites

- Python 3.x
- [Ollama](https://ollama.ai/) installed and running locally
- The following models pulled in Ollama:
  - `llama3.2` (for text generation)
  - `mxbai-embed-large` (for embeddings)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yxsh-uwu/Local-AI-Agent.git
cd Local-AI-Agent
```

2. Create and activate a virtual environment (recommended):
```bash
python -m venv venv
# On Windows
.\venv\Scripts\activate
# On Unix or MacOS
source venv/bin/activate
```

3. Install the required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Ensure Ollama is running in the background with the required models pulled

2. Run the main script:
```bash
python main.py
```

3. Enter your questions about restaurants when prompted. Type 'q' to quit.

## Project Structure

- `main.py`: The main application script with the Q&A loop
- `vector.py`: Handles vector embeddings and Chroma DB integration
- `realistic_restaurant_reviews.csv`: Dataset containing restaurant reviews
- `requirements.txt`: Lists all Python dependencies
- `chroma_langchain_db/`: Local vector database storage (automatically created)

## Dependencies

- langchain: Framework for developing LLM applications
- langchain-ollama: Integration with Ollama
- langchain-chroma: Vector store integration
- pandas: Data manipulation and CSV handling

## License

MIT License

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.