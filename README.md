# Groq QA Chatbot 

This project integrates **Groq** and **LangChain** to create a simple QA chatbot using the **Llama 3-8b model**. The chatbot takes user input and returns a response based on a series of pre-defined prompts.

## Features

- **Chatbot Interface:** The chatbot answers user questions based on a conversational AI model.
- **LangChain Integration:** Uses LangChain for processing the prompt, interacting with the Groq API, and parsing the output.
- **Environment Setup:** Uses environment variables for securely storing the `GROQ_API_KEY`.
  
## Technologies Used

- **LangChain** for creating the language model pipeline.
- **Groq API** for providing AI-driven conversation capabilities.
- **Python-dotenv** for loading environment variables from a `.env` file.

## Installation and Setup

### Prerequisites

Ensure that you have the following installed:

- Python 3.x
- pip (Python package installer)
- A Groq API key (you can get this by signing up on Groq's platform).

### 1. Clone the repository:

```bash
git clone <your_repository_url>
cd <your_repository_directory>
````

### 2. Install dependencies:

Run the following command to install the required Python libraries:

```bash
pip install langchain langchain-groq python-dotenv
```

### 3. Set up environment variables:

* Create a `.env` file in your project directory.
* Add the following variable with your Groq API key:

```env
GROQ_API_KEY=your_groq_api_key_here
```

### 4. Run the Python script:

Once everything is set up, you can run the script that starts the chatbot interface:

```bash
python chatbot.py
```

## How to Use the Chatbot

Once the chatbot is running, you can interact with it via the terminal:

1. **Ask a question**: Type a question after the prompt.
2. **Quit**: Type `quit` or `exit` to exit the chatbot.

For example:

```
You (type 'quit' or 'exit'): What is the color of the sky?
Bot: The color of the sky is typically blue.
```

### Example of Interaction:

```bash
--- Basic Groq QA Chatbot ---
The chatbot is ready. Type your question in the input box that will appear below and press Enter.
Type 'quit' or 'exit' to end the chat.
--------------------------------------------------

You (type 'quit' or 'exit'): What is the colour of the sky?
Bot: The colour of the sky is typically blue.
```

## Troubleshooting

* **Missing API Key:** Make sure your `.env` file contains the correct `GROQ_API_KEY` and is placed in the root directory.
* **Installation Issues:** Ensure that all dependencies are installed by running `pip install -r requirements.txt` if you're using a `requirements.txt` file.
* **LangChain Error:** If LangChain does not initialize properly, verify your `chat_model` and `qa_chain` configurations.

## Author

**Anvita Manne**
