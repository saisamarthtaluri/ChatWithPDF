# Chat with Your PDF

## Introduction

This Streamlit application enables users to chat directly with their PDF files, making it a breeze to ask any questions about their documents. It works by first extracting textual content from the provided PDF, then creating meaningful embeddings either through OpenAI or local HuggingFace Embeddings (note: using the latter can be slightly slower). The application then performs a semantic search based on the user's query. The semantic search results are subsequently passed to a Large Language Model (LLM) like OpenAI's ChatGPT, Llama 2 or models available on the Hugging Face Hub. The process utilizes Langchain, ensuring conversation memory is retained through Langchain's Memory Buffer. The response from the LLM is presented back to the user.

## Features

- **Document Upload**: Quickly upload multiple PDF files to chat with.
- **Multiple Embedding Support**: Choose between OpenAI or HuggingFace Embeddings.
- **Semantic Search**: Enhanced search capability that understands the context of the user's query.
- **Integration with LLMs**: Integrated with popular models like OpenAI's ChatGPT,Llama 2 and models from Hugging Face Hub.
- **Conversation Memory**: Thanks to Langchain's Memory Buffer, the application remembers the conversation, providing a cohesive chatting experience.

## Installation & Usage

1. Clone the repository:   
```
git clone https://github.com/saisamarthtaluri/ChatWithPDF.git
cd ChatWithPDF
```
2. Install the necessary libraries:
```
pip install -r requirements.txt
```
3. Add your OpenAI Key or HuggingFaceHub Token based on your requiremnts in .env file.
   
5. Modify the code (uncomment) if you don't want to use OpenAI's LLM and Embeddings.
   
7. Run the Streamlit application:
```
streamlit run app.py
```
6. Visit the Streamlit URL in your browser. Upload your PDFs using the sidebar and start chatting with your documents.

Developed with ❤️ by SaiSamarth
