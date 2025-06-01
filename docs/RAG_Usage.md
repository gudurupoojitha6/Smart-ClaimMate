Written Statement on Retrieval-Augmented Generation (RAG) and IBM watsonx.ai Usage
Smart ClaimMate uses IBM watsonx.ai combined with a Retrieval-Augmented Generation (RAG) pipeline to deliver highly contextual, accurate, and human-like responses for insurance claim support.

Our assistant was built using IBM watsonx.ai Prompt Lab, where we fine-tuned the system to:

Accept natural-language user queries related to claims, hospitals, or documents

Retrieve relevant information from uploaded knowledge files (e.g., policy PDFs, hospital plan documents)

Respond in plain, polite, and emotionally supportive language

How RAG is used in the solution:

Document Upload: We upload insurance policy documents, denial templates, and hospital listings as the retrieval source.

Prompt Configuration: Prompts are crafted to guide the assistant to only respond based on the uploaded content and avoid hallucination.

Question Handling: When a user asks a question (e.g., "Why was my claim denied?" or "Which hospital near me accepts this plan?"), the RAG pipeline:

Retrieves the most relevant text chunks from the uploaded files

Uses those snippets to generate grounded, context-specific answers

Personalization: Based on the ZIP code input by the user, Smart ClaimMate pulls hospital data from the source files to display nearby hospitals with ratings, doctor availability, wheelchair access, and estimated treatment cost.

Trust Score Generation: After a user uploads their denial letter and related documents, the assistant analyzes the content using prompt instructions and gives a predicted approval compatibility score.

watsonx.ai's role:

Used Prompt Lab for rapid testing and refinement of system prompts

Leverages watsonx's NLP capabilities to maintain polite tone, clarity, and relevance

Ensures responses are generated only from grounded, retrievable sources to maintain accuracy

The assistant is prompt-driven and can be easily updated for new industries (e.g., auto insurance or banking) by simply uploading new domain-specific files and updating system instructions—showcasing the flexibility and reusability of IBM watsonx.ai in combination with RAG.

