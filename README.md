The main logic of the RAG pipeline is in the file "rag.ipynb" file in which we :
1) Converts the pdfs into uniform langchain document format
2) Splits each document into further chunks using text_splitters (RecursiveCharacterTextSplitter)
3) Embeds every chunk created in the step 2 using a embedding model (sentence transformer("all-MiniLM-l6-v2"))
4) Store and persist the created embeddings using ChromaDB vectorStore.
