llm_resume - it is simple rag implementation
llm_resume_1 - it has sub-chain that takes the latest user question and reformulates it in the context of<br> the chat history. This can be thought of simply as building a new "history aware" retriever. Whereas before we had:<br>
query -> retriever<br>
Now we will have:<br>
(query, conversation history) -> LLM -> rephrased query -> retriever<br>
