# Doc-Query-Agent

Doc-Query-Agent is a natural language query agent tools like lang chain, chromadb, and replicate. It also implements features like conversational memory, summary providing and giving citations to the text used. Note that this implementation uses open-source tools only and can perform better by using larger LLM's like GPT-4.

## How to use
1. Put in the documents to be queried in the data folder.
2. Access the llama-2-70b chat model using your replicate API key.

## What it does
1. The input data is broken into chunks using lang chain text splitter.
2. These chunks are converted into numerical representations or embeddings using sentence-transformers open source embeddings from huggingface.
3. These embeddings are stored in a vector store, which can be queried for a similarity search.
4. The most relevant chunks, previous conversation history, and a prompt are fed into the LLM.
   


