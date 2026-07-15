# Day 4 - Using Hugging Face Models in LangChain

## 📅 Date
15 July 2026

## Objective

Learn how to use Hugging Face models in LangChain by:
- Accessing models using the Hugging Face API.
- Running models locally on my computer.

---

## Topics Covered

### 1. Using Hugging Face API

Used the `HuggingFaceEndpoint` class to access models through the Hugging Face API.

### Steps

1. Import required classes.
2. Load environment variables using `python-dotenv`.
3. Store the Hugging Face API key in a `.env` file.
4. Create an `HuggingFaceEndpoint`.
5. Specify:
   - `repo_id` (model to use)
   - `task` (e.g., `text-generation`)
6. Wrap the endpoint using `ChatHuggingFace`.
7. Call `invoke()` to generate a response.

---

### 2. Running Models Locally

Used `HuggingFacePipeline` to run models on the local machine.

### Steps

1. Import `HuggingFacePipeline`.
2. Specify:
   - `model_id`
   - `task`
3. Configure model parameters such as:
   - `temperature`
   - `max_new_tokens`
4. Wrap it using `ChatHuggingFace`.
5. Use `invoke()` to get the response.

---

## Difference

| Hugging Face API | Running Locally |
|------------------|-----------------|
| Uses API key | No API key required |
| Model runs on Hugging Face servers | Model runs on local machine |
| Requires internet | Can work offline after downloading the model |
| Faster to start | Requires downloading the model |

---

## What I Learned

- How to use Hugging Face models through LangChain.
- Difference between using the Hugging Face API and running models locally.
- How to use `HuggingFaceEndpoint`.
- How to use `HuggingFacePipeline`.
- How `ChatHuggingFace` provides a chat interface for both approaches.
- Importance of `repo_id`, `task`, `temperature`, and `max_new_tokens`.

---

## Packages Used

- langchain-huggingface
- python-dotenv
- transformers

---

## Next Topic

Prompt Templates