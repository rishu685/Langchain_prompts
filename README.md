# LangChain Prompts

A collection of LangChain examples and tools demonstrating various prompt engineering techniques and conversational AI implementations.

## Features

- **Research Paper Summarization Tool**: Interactive Streamlit app for summarizing academic papers with customizable style and length
- **Prompt Templates**: Examples of creating and using prompt templates with LangChain
- **Chat Templates**: Implementations of conversational prompts with message handling
- **Interactive Chatbot**: Command-line chatbot with conversation history
- **Temperature Control**: Examples of controlling AI model creativity through temperature settings

## Project Structure

```
├── README.md                    # This file
├── package.json                 # Project metadata
├── template.json               # Saved prompt template for research summarization
├── prompt_ui.py                # Streamlit web app for research paper summarization
├── prompt_template.py          # Basic prompt template examples
├── prompt_generator.py         # Template creation and saving utilities
├── chat_prompt_template.py     # Chat-based prompt templates
├── message_placeholder.py      # Message placeholder handling
├── messages.py                 # Direct message handling with LangChain
├── chatbot.py                  # Interactive command-line chatbot
├── temperature.py              # Temperature parameter examples
└── chat_history.txt            # Sample chat history data
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/campusx-official/langchain-prompts.git
cd langchain-prompts
```

2. Install required Python packages:
```bash
pip install langchain-openai langchain-core streamlit python-dotenv
```

3. Set up environment variables:
Create a `.env` file in the project root and add your OpenAI API key:
```
OPENAI_API_KEY=your_openai_api_key_here
```

## Usage

### Research Paper Summarization Tool

Run the Streamlit web application:
```bash
streamlit run prompt_ui.py
```

This launches an interactive web interface where you can:
- Select from predefined research papers (Attention Is All You Need, BERT, GPT-3, Diffusion Models)
- Choose explanation style (Beginner-Friendly, Technical, Code-Oriented, Mathematical)
- Set summary length (Short, Medium, Long)
- Generate customized summaries with mathematical details and analogies

### Interactive Chatbot

Run the command-line chatbot:
```bash
python chatbot.py
```

Type your messages and interact with the AI assistant. Type 'exit' to quit.

### Prompt Template Examples

Explore various prompt engineering techniques:

```bash
# Basic prompt templates
python prompt_template.py

# Chat-based templates
python chat_prompt_template.py

# Message handling
python messages.py

# Temperature control
python temperature.py
```

## Key Components

### Prompt Templates
- **Basic Templates**: Simple string-based templates with variable substitution
- **Chat Templates**: Structured conversation templates with system/human/AI message roles
- **Message Placeholders**: Dynamic message history integration

### Research Summarization
- Customizable explanation styles and lengths
- Mathematical equation handling
- Analogy-based explanations
- Template persistence with JSON serialization

### Conversation Management
- Message history tracking
- Multi-turn conversations
- System message configuration
- Context preservation

## Requirements

- Python 3.7+
- OpenAI API key
- Required packages:
  - `langchain-openai`
  - `langchain-core`
  - `streamlit`
  - `python-dotenv`

## Contributing

Feel free to contribute by:
1. Adding new prompt examples
2. Improving the research summarization tool
3. Adding new conversation templates
4. Enhancing documentation

## License

ISC License

## Repository

- **GitHub**: [langchain-prompts](https://github.com/campusx-official/langchain-prompts)
- **Issues**: [Report bugs or request features](https://github.com/campusx-official/langchain-prompts/issues)

---

This project demonstrates practical applications of LangChain for prompt engineering, making it easier to understand and implement conversational AI systems with customizable prompts and templates.