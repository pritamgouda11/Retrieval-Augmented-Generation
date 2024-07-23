# RAG-based Document Insights Generator

![Logo]([path_to_logo_image](https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2F%40nikita04%2Fwhat-is-rag-retrieval-augmented-generation-7875ce0de5b1&psig=AOvVaw1EZm6xLjGNyvip9A2VxS5c&ust=1721807443666000&source=images&cd=vfe&opi=89978449&ved=0CBAQjRxqFwoTCJCVu9rWvIcDFQAAAAAdAAAAABAI))

Welcome to the **RAG-based Document Insights Generator**! This project leverages Retrieval-Augmented Generation (RAG) using Streamlit and various NLP models to provide insights from your uploaded documents. It integrates multiple document loaders and state-of-the-art NLP models to create an interactive platform for querying document content.

## What is Retrieval-Augmented Generation (RAG)?

Retrieval-Augmented Generation (RAG) is a method that combines retrieval-based techniques with generative models. It enhances the ability to generate accurate and contextually relevant responses by retrieving relevant information from a large corpus of documents and feeding it into a generative model.

![RAG Architecture](![image](https://github.com/user-attachments/assets/59c295ea-ccc6-4fc6-ab4f-e66e05159b11)
)

### How RAG Works

1. **Document Retrieval**: The system retrieves relevant chunks of text from a document database based on the user's query.
2. **Response Generation**: The retrieved text is then used to generate a detailed and contextually accurate response using advanced language models.

![RAG Workflow](![image](https://github.com/user-attachments/assets/9c905c4a-9cf8-4e0c-ac3e-56a2bab80a83)
)

## Features

- **Multi-Format Document Support**: Upload PDFs, CSVs, and text files.
- **Efficient Text Processing**: Documents are split into manageable text chunks for better processing.
- **Robust Vector Store Creation**: Create and update vector stores for efficient document retrieval.
- **Conversational AI**: Ask questions and get insights from your documents using advanced NLP models.

## How It Works

1. **Upload Documents**: Use the sidebar to upload your documents.
2. **Process Documents**: Click the "Process" button to parse and store document content.
3. **Ask Questions**: Enter your queries in the main interface to get insights from your documents.

## Technologies Used

- **Streamlit**: For the interactive web interface.
- **Langchain**: For creating document chains and managing conversational AI.
- **Chroma**: For vector store creation and retrieval.
- **OpenAI & Cohere**: For embeddings and language models.

## Installation

1. **Clone the Repository**
    ```sh
    git clone https://github.com/yourusername/your-repo.git
    cd your-repo
    ```

2. **Install Dependencies**
    ```sh
    pip install -r requirements.txt
    ```

3. **Set Up Environment Variables**
    Create a `.env` file in the root directory and add the following:
    ```env
    PERSIST_DIRECTORY=path_to_persist_directory
    SOURCE_DIRECTORY=source_documents
    TARGET_SOURCE_CHUNKS=5
    EMBEDDINGS_MODEL_NAME=openai
    MODEL_TYPE=OpenAI
    ```

4. **Run the Application**
    ```sh
    streamlit run app.py
    ```

## Usage

1. **Upload Documents**
    - Supported formats: PDF, CSV, Text
    - Upload documents via the sidebar.

2. **Process Documents**
    - Click the "Process" button to parse and vectorize the documents.

3. **Ask Questions**
    - Use the text input box to ask questions about the uploaded documents.
    - The system will retrieve relevant information and generate insightful responses.

## Screenshots

![Upload Documents](path_to_screenshot1)
*Upload your documents via the sidebar.*

![Ask Questions](path_to_screenshot2)
*Enter your questions and get insightful answers.*

## Customization

- **Embeddings and Models**: Customize the embeddings model and the conversational AI model by modifying the environment variables.
- **Chunk Size and Overlap**: Adjust the text chunk size and overlap parameters to optimize processing.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License.

## Acknowledgments

- **OpenAI** for their powerful language models.
- **Streamlit** for making data apps simple and accessible.
- **Langchain and Chroma** for their amazing tools and libraries.

---

Feel free to reach out for any questions or support!

![Footer Image](path_to_footer_image)
