# Building-a-Football-Chatbot-with-RAG

## **Generalities**
This assignment involves building a chatbot capable of answering questions about football (soccer) based on a dataset of articles from *Les Cahiers du Football*, a French website specializing in in-depth football analysis. The chatbot will utilize a Retrieval-Augmented Generation (RAG) architecture to provide accurate, grounded answers in English, despite the source material being in French. The chatbot will also identify and cite its sources and admit when it cannot provide a relevant answer.

## **Objective**
The goal is to create a smart chatbot that:

* Accepts queries in English and provides responses in English.

* Searches through the provided dataset of football articles for relevant information.

* Returns answers grounded in the dataset, along with citations (article titles or URLs), using LLMs.

* Recognizes when no relevant information exists and responds with "I don't know."

## **Data**
The dataset consists of approximately 10,000 articles from Les Cahiers du Football. Each article has been split into chunks of around 400 words and embedded into a Milvus vectorstore using cosine similarity for efficient retrieval. Metadata for each chunk includes: *Article ID*, *Title* and *URL*.
