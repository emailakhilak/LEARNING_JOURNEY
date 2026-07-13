# Day 2 - Understanding Models in LangChain

## Date

13 July 2026

## Objective

Learn the different types of models available in LangChain and understand when to use **LLMs** and **Chat Models**.

---

## Topics Covered

### Large Language Models (LLMs)

understood how the **closed-source LLMs** works using API keys.

Examples:

* OpenAI GPT models (Completion APIs)

LLMs are designed for **single text generation tasks** such as:

* Text generation
* Summarization
* Translation
* Question answering
* Content completion

---

### Chat Models

Understood how the **closed-source Chat Models** works using API keys.

Examples:

* OpenAI Chat Models
* Google Gemini
* Anthropic Claude

Chat Models are optimized for **multi-turn conversations** and understand the context of previous messages provided in the conversation history.

---

# LLMs vs Chat Models

| Feature              | LLM                                                             | Chat Model                                                             |
| -------------------- | --------------------------------------------------------------- | ---------------------------------------------------------------------- |
| Primary Purpose      | Single text generation                                          | Multi-turn conversations                                               |
| Input Format         | Plain text prompt                                               | List of messages (System, Human, AI)                                   |
| Conversation Context | No built-in conversation structure                              | Designed to work with conversation history                             |
| Roles                | Not supported                                                   | Supports System, Human, and AI roles                                   |
| Best Use Cases       | Summarization, text completion, translation, content generation | Chatbots, AI assistants, customer support, conversational applications |

---

## Examples

### Example 1 – Text Summarization (LLM)

**Prompt**

> Summarize the following paragraph in three sentences.

**Output**

The model returns only the summarized text.

This is a typical use case for an LLM because only a single prompt is required.

---

### Example 2 – Chatbot (Chat Model)

**Conversation**

**System**

> You are a helpful programming tutor.

**Human**

> Explain what LangChain is.

**AI**

> LangChain is a framework for building applications powered by large language models.

**Human**

> Can you explain it with an example?

The chat model understands the previous conversation and generates a response based on the conversation history.

---

## Key Takeaways

* LLMs are best suited for single text-based tasks such as text generation, summarization, translation, and content completion.
* Chat Models are designed for conversational AI and work with structured messages.
* Chat Models support different message roles such as **System**, **Human**, and **AI**, allowing better control over model behavior.
* Building chatbots, AI assistants, and agents is generally easier with Chat Models due to their conversation-oriented interface.

---
