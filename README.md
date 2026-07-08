# Local AI Chatbot with Ollama

A privacy-first, multimodal AI chatbot that runs entirely on your machine using Ollama and Gradio. 

---

## Features

- **Intelligent Conversations** — Natural, context-aware chat with local LLMs
- **Image Understanding** — Upload images and ask questions about them (multimodal)
- **File Processing** — Upload text/code files for analysis and discussion
- **100% Private** — All processing happens locally, zero data sent anywhere
- **Clean Web Interface** — User-friendly chat UI built with Gradio
- **Offline Ready** — No internet needed after initial model download
- **Error Handling** — Graceful handling of connection issues, missing models, and input errors

---

## Prerequisites

| Software | Required For | Download |
|----------|-------------|----------|
| **Python 3.10+** | Running the chatbot code | [python.org](https://python.org) |
| **Ollama** | Running AI models locally | [ollama.ai](https://ollama.ai) |

> **Windows Users:** Check **"Add Python to PATH"** during Python installation

---

## Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/ollama-chatbot.git
cd ollama-chatbot
### 2. Set Up Virtual Environment
```Windows:

cmd
python -m venv chatbot_env
chatbot_env\Scripts\activate
Mac/Linux:

bash
python3 -m venv chatbot_env
source chatbot_env/bin/activate
3. Install Dependencies
cmd
pip install -r requirements.txt
4. Pull AI Models
cmd
# Required: Text chat model (~1.5GB)
ollama pull llama3.2:1b

# Optional: Image understanding model (~4GB)
ollama pull llava:7b
5. Start Ollama Service
Open a new terminal and run:

cmd
ollama serve
Keep this terminal running in the background.

6. Launch the Chatbot
In your first terminal (with virtual environment activated):

cmd
python basic_chatbot.py
7. Access the Chatbot
Open any web browser (Chrome, Firefox, Edge, Safari)

Go to: http://127.0.0.1:7860

The chat interface will appear with a text box

Type your message and press Enter to start chatting

The AI will respond within a few seconds

Your private AI assistant is now ready to use.
