# AI Research Assistant Agent

![Project Banner](placeholder-banner.png)

A Python-based AI research assistant agent that leverages LangChain to interact with LLMs (GPT/Claude), perform web searches, query Wikipedia, and saves structured research outputs to files.

## Features

- **Multi-LLM Support**: Works with both OpenAI GPT and Anthropic Claude models
- **Tool Integration**: 
  - Web search via DuckDuckGo
  - Wikipedia lookups
  - Custom file saving functionality
- **Structured Outputs**: Returns research in consistent, programmatically accessible formats
- **Interactive**: Accepts user queries via command line input

## Prerequisites

- Python 3.10+
- [Visual Studio Code](https://code.visualstudio.com/) (recommended)
- API keys for:
  - [OpenAI](https://platform.openai.com/api-keys) or 
  - [Anthropic](https://console.anthropic.com/settings/keys)

## Setup

1. **Create Project Folder**
```bash
   mkdir ai-agent-tutorial
   cd ai-agent-tutorial
   ```

2. **Set Up Virtual Environment and activate it**   
```bash
python -m venv venv
.\venv\Scripts\activate

if you are using a Mac, use the script below:
source venv/bin/activate
```
3. **Install Dependencies**
paste the following in a file named requirements.txt in your VSCode environment
```bash
langchain
wikipedia
langchain-community
langchain-openai
langchain-anthropic
python-dotenv
pydantic
duckduckgo-search
```
run the script below
```bash
pip install -r requirements.txt
```

## Configuration
1. **Create .env file:** We are going to create a .env file and paste our Open API or Claude API key there, I will be using Claude in my own environment
```bash
# For OpenAI
OPENAI_API_KEY=your_key_here

# For Anthropic
ANTHROPIC_API_KEY=your_key_here
```

## Usage

1. **Run the agent:**
```bash
python \main.py
```


2. **Enter your research query when prompted:**
```bash
What can I help you research? Tell me about quantum computing
```

The agent will:

-Search for information

-Structure the response

-Save to a timestamped text file

![Output](images/Screenshot%20(1097).png)

### See the images folder for more details
