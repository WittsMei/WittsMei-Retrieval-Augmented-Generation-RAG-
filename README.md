# WittsMei-Retrieval-Augmented-Generation-RAG-

### Retrieval augmented generation (RAG) 
- Retrieval augmented generation (RAG) is a technique for improving the quality of LLM output by grounding it with sources of knowledge not available in the trained model.

- With RAG, you modify the prompt to provide extra data, including **proprietary data**, to the model. No fine tuning of the model is required. For example, Gemini has been trained against public data, so your organization's knowledge bases and other private data is not a part of the Gemini model.

- RAG provides the model with access to information retrieved from trusted knowledge bases or documents, which improves accuracy of responses. This information can include proprietary data that is not in the model, as well as sensitive user-specific data that should never be put into a training model.


### An example of how the RAG technique is used to enhance the response from an LLM
1. Data retrieval
An LLM typically does not include user data when it is being trained. **User data is dynamic**, which usually means that a trained LLM cannot have the most up-to-date data. More importantly, **user data is sensitive**, and you do not want an LLM to be able to provide user data to a different user in its responses.

   In addition, **foundation models are not trained with proprietary data**, like knowledge bases and document stores. For example, when you send a prompt directly to Gemini, you cannot ask Gemini for information that is not    available on the internet.

   This data can be retrieved and provided to the model as part of the prompt.

2. Augmented prompt
In addition to the user's query and the guidance provided to the model, the prompt is augmented with the retrieved data. The prompt instructs the model to trust the retrieved data, and the model can also be asked to ground the data by providing references or links to the data so the user can access the full document.

3. Generated response
The model uses all of the information in the prompt (including the retrieved data) to generate the response.
<img width="1276" height="554" alt="791af063-ca05-4193-bc83-2c9a81140205" src="https://github.com/user-attachments/assets/e185ea73-59ff-45ea-a66d-7d8be416a3dc" />

### Retrieving data for RAG

- The "retrieval" in retrieval augmented generation allows the model to use data that is not available in the model itself. RAG is typically used to provide two types of data to the model in the prompt:

- User data: For a chatbot this is the data associated with the user providing the query.
Other data not available in the model: For a chatbot this often includes knowledge base data or relevant documents that are not available on the internet.

### Retrieving relevant data: Semantic search
- **Semantic search** attempts to provide results that are guided by the meaning of the query, not by directly matching the words in the query.
- Traditionally, most searches performed by applications have been keyword searches. A keyword search looks for text matches to find matching content. For example, in a database, you might search for a category with one or more specific values:
  <img width="1540" height="242" alt="560105e5-594a-4793-bf5a-d8a466b770e4" src="https://github.com/user-attachments/assets/4bc48a36-a7e9-478b-bfb5-3a5818ebf603" />


### Retrieving relevant data: Vector search
- Vector search uses vectors (lists of numbers) to represent and search content.
- Three steps: 1. Encode the data   2. Index the data   3. Search the data





