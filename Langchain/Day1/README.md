DAy1- Introduction to Langchain
07-07-2026

Langchain is an opensource framework for developing application powered by llm

Benifits
-> handles workflow pippeline(one component output is the input of another - this can be done automatically)
-> componets with many variations are available
-> Easy shifing between componets
-> Memory state handling example like the way the chatgpt can able to remember previous messages

What can we build
->Conversational chatbots - helpful for service centers
->AI Agents - helpful to do the works like booking flights
->Summarization - in chatgpt we cannot upload huge info but throught langchain we ca build a chatbot that can take huge info and answers your question

Components of Langchain
-> Model - interface to interact with ai models
-> Prompts - which is given as input to llms
-> chain - pipeline
-> Memory - llm APIs are stateless(cannot remember messages from previous apis)can be solved by langchain
-> Indexex - 4 main components - Document loader,text splitter,vector store,retrivers - from the chat with pdf application example
-> Agents


story time

we want to build a chatbot

At first, we face two big problems:

The chatbot should understand what the user is asking (NLU).
It should give a correct answer using the available context (context-aware text generation).

For many years, these were difficult problems.

Then LLMs (like GPT) came and solved both of them. Now the chatbot can understand questions and generate good answers.

But a new problem appeared.

These LLMs are very large. Running them on our own server needs expensive GPUs, lots of memory, and high maintenance costs.

So instead of hosting the model ourselves, companies like OpenAI provide LLM APIs.

Now we simply send a request to the API, and it returns the answer. We don't have to manage the model ourselves.

Again, another problem appeared.

A chatbot is not just an LLM.

It also needs:

A document loader
A text splitter
An embedding model
A vector database
An LLM API
Prompt management
Memory
Retrieval logic

Connecting all these parts and making them work together is complicated. If we want to switch from OpenAI to Gemini or change the vector database, we may have to modify a lot of code.

Then LangChain came to solve this problem.

LangChain acts like a manager. It connects all these components together using a common interface.

Because of this:

You write less code.
You can change one component (like the LLM or vector database) with only a few changes.
You can focus on building your chatbot instead of worrying about connecting everything.


LLMs solved intelligence.
LLM APIs solved hosting.
LangChain solved orchestration (connecting everything together).