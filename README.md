# AI Agent with Document Memory
This repository contains code for an AI Agent with Document Memory, which can answer questions about the input document using the OpenAI GPT-4 model.

## Introduction
The AI Agent with Document Memory is built using various Python libraries and tools to provide intelligent question-answering capabilities based on the context and memory available. The agent uses the OpenAI GPT-4 model for language understanding and answering questions.

## Features
1. Utilizes the OpenAI GPT-4 model for natural language processing.
2. Supports parsing PDF files and extracting text content from them.
3. Splits large documents into smaller chunks to facilitate question-answering.
4. Indexes the document chunks using FAISS for efficient retrieval.
5. Provides a conversation-based interface for asking questions to the agent.
6. Memory feature allows the agent to retain past conversation context.

## How to Use
1. First, you need to set up your OpenAI API key. If you don't have one, you can sign up on the OpenAI website to obtain an API key.
2. Install the required dependencies.
3. Place your PDF file in the desired location and update the pdf_file_path variable in the code with the correct path.
4. Run the test_embed() function to parse the PDF, convert it into document chunks, and create an index using the OpenAI GPT-4 embeddings.
5. The qa object allows you to interact with the agent using a single tool that performs question-answering based on the indexed documents.
6. The agent is configured to have a conversation with a human. You can interact with the agent using the agent_chain.run(query) function, where query is the question you want to ask.


## Notes
The OpenAI GPT-4 model is used with a temperature setting of 0 to make the responses more deterministic.
Feel free to experiment with different parameters and settings to fine-tune the agent's performance based on your specific use case.


## Acknowledgements
This project was made possible with the help of the OpenAI GPT-4 model and other open-source libraries.
Special thanks to the developers of the langchain library for providing useful tools for natural language processing tasks.

