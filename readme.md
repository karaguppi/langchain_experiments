# Chat with a Website from URL - LangChain Chatbot with Streamlit GUI

Welcome to the GitHub repository for the LangChain Chatbot with Streamlit GUI! This project is a comprehensive guide to building a chatbot capable of interacting with websites, extracting information, and communicating in a user-friendly manner. It leverages the power of LangChain 0.1.5 and integrates it with a Streamlit GUI for an enhanced user experience.

## Features
- **Website Interaction**: The chatbot uses the latest version of LangChain to interact with and extract information from various websites.
- **Large Language Model Integration**: Compatibility with models like GPT-4, Mistral, Llama2, and ollama. In this code I am using GPT-3.5 and Text-embeddings-ad-002 for embeddings model, but you can use which ever model you have access to. 
- **Streamlit GUI**: A clean and intuitive user interface built with Streamlit, making it accessible for users with varying levels of technical expertise.
- **Python-based**: Entirely coded in Python.
- **Tracing-with-Langsmtih**: This entire code block is traced to Langsmith which is currently in beta. This allows us ease of debugging and cost tracking as well as visibility over key performance metrics of the models being used. Check out the official documentation to get started with LangSmith. 

## Brief explanation of how RAG works

A RAG bot is short for Retrieval-Augmented Generation. This means that we are going to "augment" the knowledge of our LLM with new information that we are going to pass in our prompt. We first vectorize all the text that we want to use as "augmented knowledge" and then look through the vectorized text to find the most similar text to our prompt. We then pass this text to our LLM as a prefix.

For a more in-depth walk-through, you can go to the official LangChain documentation.


## Installation
Ensure you have Python installed on your system. Then clone this repository:

```bash
git clone [repository-link]
cd [repository-directory]
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Create your own .env file with the following variables:

```bash
OPENAI_API_KEY=[your-openai-api-key]
```
Do not forget to add these to .gitignore files or set these up as secrets in your environment. 
## Usage
To run the Streamlit app:

```bash
streamlit run app.py
```

## Contributing
If you find any bugs or cool features you would like to add, please create a feature branch with your username and raise a PR so that I can view. I can either integrate it to this branch or make it standalone application with added features. 

---
Thanks for checking this out! 