# Steps_ai assignment
Project Overview
This project focuses on developing a sophisticated information retrieval and question-answering system. The system involves web crawling, data chunking, embedding creation, vector database indexing, retrieval, re-ranking, and question answering. It utilizes advanced techniques to ensure accurate and efficient retrieval of relevant information.

ey Features
Data Collection and Cleaning
Web Crawling: The project begins with scraping data from specified web sources.
HTML Parsing: The scraped HTML content is cleaned and parsed to extract plain text using BeautifulSoup.
Data Chunking
Advanced Chunking: The cleaned text is split into meaningful chunks based on sentence and topic similarity, avoiding naive chunking methods.
Chunk Size Management: Each chunk is managed to ensure it falls within a specified size limit for optimal processing.
Embedding Creation
Embeddings: The text chunks are converted into embedding vectors using a pre-trained language model from Hugging Face's transformers library.
Vector Database Creation
FAISS Indexing: Instead of Milvus, the project uses FAISS (Facebook AI Similarity Search) to create a vector database.
HNSW Indexing: Embedding vectors are indexed using the HNSW (Hierarchical Navigable Small World) method for efficient similarity search.
Metadata Storage: Relevant metadata, such as web links of the extracted chunks, are stored alongside the vectors in the database.
Retrieval and Re-ranking
Hybrid Retrieval: The system employs hybrid retrieval methods combining traditional BM25 with modern BERT-based retrieval techniques.
Query Expansion: Advanced query expansion techniques are used to enhance the retrieval process.
Re-ranking: Retrieved results are re-ranked based on their relevance and similarity to the query.
Question Answering
Language Model Integration: The top re-ranked chunks are passed to a language model for generating accurate and relevant answers.
Contextual Richness: The system ensures that the combined context from relevant chunks provides a comprehensive background for the language model to generate precise answers.
User Interface (Optional)
Interactive Interface: An optional user interface can be created using frameworks like Streamlit or Gradio, allowing users to input queries and receive answers in a user-friendly manner.
Conclusion
This project combines state-of-the-art techniques in natural language processing and information retrieval to create a robust question-answering system. It leverages advanced methods for data chunking, embedding creation, vector database indexing, and hybrid retrieval, ensuring efficient and accurate information retrieval and answering.

