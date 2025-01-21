# Constitution of India Question Answer Document
   Provides an overview of the project, explaining that it is a Streamlit-based app using Retrieval Augmented Generation (RAG) for answering questions about the Constitution of India.
## Workflow 
   1.Source documents are loaded by PyPDFDirectoryLoader

   2.Documents are split into small size by RecursiveCharacterTextSplitter

   3.Each document chunk is converted into a dense vector representation by GoogleGenerativeAIEmbeddings
   
   4.These chunks are stored in the vector database FAISS

   5.User given a prompt through an interface Streamlit and these are processed by the above steps and passed to the Language Model which generate answer
   
   
