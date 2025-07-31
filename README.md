# WittsMei-Retrieval-Augmented-Generation-RAG-

### Retrieval augmented generation (RAG) 
- Retrieval augmented generation (RAG) is a technique for improving the quality of LLM output by grounding it with sources of knowledge not available in the trained model.

- With RAG, you modify the prompt to provide extra data, including **proprietary data**, to the model. No fine tuning of the model is required. For example, Gemini has been trained against public data, so your organization's knowledge bases and other private data is not a part of the Gemini model.

- RAG provides the model with access to information retrieved from trusted knowledge bases or documents, which improves accuracy of responses. This information can include proprietary data that is not in the model, as well as sensitive user-specific data that should never be put into a training model.


### An example of how the RAG technique is used to enhance the response from an LLM
-  1. Data retrieval
An LLM typically does not include user data when it is being trained. **User data is dynamic**, which usually means that a trained LLM cannot have the most up-to-date data. More importantly, **user data is sensitive**, and you do not want an LLM to be able to provide user data to a different user in its responses.

In addition, **foundation models are not trained with proprietary data**, like knowledge bases and document stores. For example, when you send a prompt directly to Gemini, you cannot ask Gemini for information that is not available on the internet.

This data can be retrieved and provided to the model as part of the prompt.

-  2. Augmented prompt
In addition to the user's query and the guidance provided to the model, the prompt is augmented with the retrieved data. The prompt instructs the model to trust the retrieved data, and the model can also be asked to ground the data by providing references or links to the data so the user can access the full document.

-  3. Generated response
The model uses all of the information in the prompt (including the retrieved data) to generate the response.
<img width="1276" height="554" alt="791af063-ca05-4193-bc83-2c9a81140205" src="https://github.com/user-attachments/assets/e185ea73-59ff-45ea-a66d-7d8be416a3dc" />

