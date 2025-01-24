# Conversational RAG with PDF Uploads and Chat History

This project is a **Conversational Retrieval-Augmented Generation (RAG) system** built using **Streamlit**, **LangChain**, **Groq**, and **HuggingFace Embeddings**. The application allows users to upload PDF files, which are processed and indexed for easy retrieval. Using a conversational interface, users can ask questions, and the system answers based on the content of the uploaded PDFs and previous conversation history.

## Features

- **PDF Upload**: Users can upload one or multiple PDF files.
- **Conversational AI**: Users can ask questions based on the uploaded PDFs, and the system responds with relevant answers.
- **Chat History Awareness**: The system uses a history-aware retrieval chain to ensure the conversation remains contextually relevant.
- **Vector Storage**: The text from the PDFs is split and embedded, stored in **Chroma** vector database for efficient retrieval.
- **Groq API**: Utilizes Groq's LLM to process and generate responses based on user input.

## Technologies Used

- **Streamlit**: Web framework for creating interactive applications.
- **LangChain**: Library for building AI-powered applications by linking LLMs and external data.
- **Groq**: Optimized inference for language models.
- **HuggingFace**: For embeddings using pre-trained models.
- **Chroma**: Vector database for fast similarity search.
- **PyPDF**: For extracting text from PDF files.
- **TensorFlow**: Machine Learning framework (used for embeddings).

## Getting Started

### Prerequisites

- Python 3.7+
- A Groq API key (required for AI inference)
- Environment variables configured (e.g., `HF_TOKEN`, `GROQ_API_KEY`)

### Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/fazil6126912/RAG-Q-A-with-conversation-history.git
    ```

2. Create a virtual environment (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up environment variables:
    - Create a `.env` file in the project directory and add:
      ```
      HF_TOKEN=your_huggingface_token
      GROQ_API_KEY=your_groq_api_key
      ```

### Running the Application

To run the Streamlit app:
```bash
streamlit run app.py
