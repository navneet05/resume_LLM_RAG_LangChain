llm_resume - it is simple rag implementation<br>
llm_resume_1 - it has sub-chain that takes the latest user question and reformulates it in the context of the chat history. <br>whereas before we have:<br>
query -> retriever<br>
Now we will have:<br>
(query, conversation history) -> LLM -> rephrased query -> retriever<br>
