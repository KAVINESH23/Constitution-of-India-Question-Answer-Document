# Constitution of India Question Answer Document
   Provides an overview of the project, explaining that it is a Streamlit-based app using Retrieval Augmented Generation (RAG) for answering questions about the Constitution of India.
## Workflow 
   -Source documents are loaded by PyPDFDirectoryLoader
   -Documents are split into small size by RecursiveCharacterTextSplitter
   Each document chunk is converted into a dense vector representation by GoogleGenerativeAIEmbeddings
   These chunks are stored in the vector database FAISS
   User given a prompt through an interface Streamlit and these are processed by the above steps and passed to the Language Model which generate answer
   
   
