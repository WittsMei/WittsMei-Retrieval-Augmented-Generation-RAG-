# WittsMei-Retrieval-Augmented-Generation-RAG-

- A powerful method for improving your responses is retrieval augmented generation(opens in a new tab), also referred to as RAG. With RAG, you modify the prompt to provide extra data to the model. No fine tuning of the model is required.

- This extra data can include **proprietary data** that is not part of the foundation model. For example, Gemini has been trained against public data, so your organization's knowledge bases and other private data is not a part of the Gemini model.

- You can also safely provide sensitive user data for the logged-in user to the model in the prompt. You do not want any other user's data to be available to the model, and there is no way for the model to access that data if it is not part of the model and it is not provided in the prompt.
