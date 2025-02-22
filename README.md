# Paul Gamma Essay Chatbot

This project is a Retrieval-Augmented Generation (RAG) chatbot that answers questions about "The Paul Gamma Essay." It uses **LlamaIndex** for document retrieval, **Google Gemini API** for response generation, and **Streamlit** for the chat interface. The chatbot retrieves relevant information from the essay and generates accurate responses using a large language model.


## Features
- **Document Retrieval**: Uses LlamaIndex to index and retrieve relevant sections from "The Paul Gamma Essay."
- **Response Generation**: Leverages Google Gemini API for generating human-like responses.
- **Streamlit Chat Interface**: Provides a user-friendly web app for interacting with the chatbot.
- **RAG Pipeline**: Combines retrieval and generation for accurate and context-aware responses.

## Prerequisites
Before running the project, ensure you have the following:
- Python 3.8 or higher
- A Google Gemini API key (sign up [here](https://ai.google.dev/))
- Basic knowledge of Python and Streamlit


## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/AndrewMarfo/paul-chat.git
   cd paul-gamma-chatbot
   ```

2. **Install Dependencies**:
    Install uv to create your environment and install dependencies
    ```bash
    pip install uv
    uv sync
    ```

## Usage
1. **Set Up Google Gemini API**:
- Create a Google Gemini API key (sign up [here](https://ai.google.dev/ ))
- Create a .env file in the root directory and add your API key as follows:
    ```bash
    api_key=YOUR_API_KEY
    ```

2. **Run the Chatbot**:
- Ensure that the `paul_graham_essay.txt` file is in the data directory.
- Run the chatbot using Streamlit:
    ```bash
    uv run streamlit run app.py
    ```
3. **Interact with the Chatbot**:
- Open a the url provided in the terminal usually `http://localhost:8501/`
- Start a conversation with the chatbot by typing in the input box.
- The chatbot will respond based on the context of the conversation.


## Technology Stack
- [LlamaIndex](https://github.com/run-llama/llama_index) - For providing the RAG pipeline and document retrieval capabilities.
- [Google Gemini API](https://ai.google.dev/) - For enabling powerful response generation using their large language model.
- [Streamlit](https://streamlit.io/) - For making it easy to build and deploy the chatbot's user interface.


Access PaulChat Application [here](https://paul-chat.streamlit.app/).