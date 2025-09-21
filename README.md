# Jane Austen RAG Retriever

This project implements a Retrieval-Augmented Generation (RAG) pipeline using LangChain and OpenAI.  
It downloads Jane Austen's novels (*Pride and Prejudice*, *Sense and Sensibility*, and *Emma*) from Project Gutenberg, splits them into chunks, stores them in vector databases, and retrieves relevant passages to answer user questions.  

## Features
- Automatic download of novels from Project Gutenberg
- Text chunking with LangChain's RecursiveCharacterTextSplitter
- Separate vectorstores for each novel
- Query routing: directs questions to the most relevant novel
- Multi-query expansion to improve retrieval quality
- RAG pipeline with context-aware answers

## Example
**Question:**  
- *"What are Elizabeth's opinions about love and courtship?"*  

**Answer (generated):**  
The system retrieves relevant passages from *Pride and Prejudice* and provides a synthesized response based on them.

- *"Elizabeth seems to have a more practical and realistic view of love and courtship. She acknowledges that Lydia's behavior is shocking and lacks decency and virtue, but also recognizes that Lydia is young and has been influenced by her surroundings. Elizabeth understands that Wickham's charm and charisma can captivate a woman, but she also seems to have a more grounded perspective on the nature of love and relationships."*
