# PDFAssistant: A Streamlit-Powered PDF Question Answering Tool
**PDFAssistant** is a tool designed to assist users in extracting and answering questions from PDF documents. Utilizing language processing models, PDFAssistant makes it easier to navigate through and understand complex documents by directly answering questions based on the content of uploaded PDFs.

## Features
**PDF Document Ingestion:** Upload one or multiple PDF documents and prepare them for querying.

**Interactive Q&A Interface:** Ask questions and receive answers directly derived from the content of the uploaded PDFs.

**Advanced Language Understanding:** Powered by the ChatOllama model and Chroma vector storage for efficient document retrieval and understanding.

## Installation
Before running PDFAssistant, ensure you have Python and Streamlit installed. Additionally, dependencies from the langchain_community package must be met. Follow these steps to set up your environment:

Clone the repository or download the source code.
Navigate to the project directory in your terminal.
Install required packages:

```bash
pip install streamlit langchain_community
```

## Usage
To use PDFAssistant, execute the Streamlit application by running the following command in the terminal from the project directory:

```bash
streamlit run app.py
```

This command will start the Streamlit server and open the application in your default web browser.

## Uploading PDF Documents
Use the "Upload document" button to select and upload the PDF documents you want to analyze.
The application will ingest the documents and prepare them for querying.

## Asking Questions
Enter your question in the "Message" input field.
The application will provide answers based on the content of the uploaded PDFs.
Resetting the Application
To clear the current session, including uploaded documents and the Q&A log, simply refresh the browser page.

## Technical Overview
app.py: The Streamlit application interface, handling document uploads, user queries, and displaying answers.
rag.py: Contains the PDFAssistant class, which manages document ingestion, query processing, and interfacing with the ChatOllama model and Chroma vector storage.

## Dependencies
- streamlit
- langchain
- pypdf
- streamlit-chat
- chromadb
- fastembed

## Limitations
Currently supports PDF documents only.

Performance may vary based on the complexity of the document and the nature of the questions.

For more information, questions, or contributions, please refer to the project's repository or contact the maintainers.

## Aknowledgements
Code based on Duy Huynh's tutorial on Medium: https://medium.com/@vndee.huynh/build-your-own-rag-and-run-it-locally-langchain-ollama-streamlit-181d42805895
