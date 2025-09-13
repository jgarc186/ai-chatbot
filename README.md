# AI Chatbot 

A simple Python chatbot that uses the OpenAI API to create a pirate-themed conversational AI assistant.

## Features

- Interactive command-line chat interface
- Pirate-themed AI assistant personality
- Maintains conversation history during the session
- Uses OpenAI's GPT-4.1-mini model for responses

## Prerequisites

- Python 3.13 or higher
- OpenAI API key
- [uv](https://docs.astral.sh/uv/getting-started/installation/) package manager

## Installation

### Install uv (if not already installed)
If you don't have uv installed, follow the installation guide at: https://docs.astral.sh/uv/getting-started/installation/

### Project Setup
1. Clone or download this repository
2. Install dependencies using uv:
   ```bash
   uv sync
   ```
3. Create a `.env` file in the project root and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```

## Usage

Run the chatbot:
```bash
uv run chatbot.py
```

The chatbot will greet you with a pirate-themed message and wait for your input. Simply type your messages and press Enter to chat with the AI assistant. The assistant will respond in character as a pirate.

To exit the chat, type `exit` and press Enter.

## Example Conversation

```
assistant: Arrgh, how can I help you, matey?

User: What's the weather like?
