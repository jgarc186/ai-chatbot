# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a simple Python chatbot project that uses the OpenAI API to create a pirate-themed conversational AI assistant. The main application is contained in a single file (`chatbot.py`) and uses the OpenAI library for API interactions.

## Development Commands

### Environment Setup
```bash
# Install dependencies using uv
uv sync

# Create a .env file with your OpenAI API key
echo "OPENAI_API_KEY=your_api_key_here" > .env
```

### Running the Application
```bash
# Run the chatbot
python chatbot.py
```

### Dependencies
- Python 3.13+
- OpenAI API library (>=1.107.2)
- python-dotenv for environment variable management

## Architecture

The application is a straightforward command-line chatbot with the following structure:

- **Single-file architecture**: All functionality is contained in `chatbot.py`
- **OpenAI integration**: Uses OpenAI's `responses.create()` method with the `gpt-4.1-mini` model
- **Environment configuration**: API keys loaded from `.env` file using python-dotenv
- **Conversation state**: Maintains conversation history in memory during the session
- **Character prompt**: Configured with a system message to make the assistant respond as a pirate

## Key Implementation Details

- The conversation history is maintained as a list of role-based messages (developer, assistant, user)
- The initial system prompt sets the pirate character behavior
- User input loop continues until "exit" is entered
- Temperature is set to 0 for consistent responses