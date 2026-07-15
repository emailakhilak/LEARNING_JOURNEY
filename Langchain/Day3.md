# Day 3 - Open Source vs Closed Source Models

## 📅 Date

14 July 2026

## Objective

Learn the differences between open source and closed source language models.

---

## Open Source Models

Open source models are models whose weights are publicly available.

Examples:

* Llama
* Qwen
* Mistral
* Gemma

### Advantages

* Can be downloaded and run locally.
* Can be fine-tuned for specific tasks.
* Can be modified and deployed on your own system.
* Better privacy when run locally because your data stays on your machine.
* No API key is required if running locally.

### Disadvantages

* Require good hardware for larger models.
* You are responsible for deployment and maintenance.

---

## Closed Source Models

Closed source models are owned by companies and are accessed through APIs.

Examples:

* OpenAI GPT
* Google Gemini
* Anthropic Claude

### Advantages

* Easy to use with an API.
* No need for powerful local hardware.
* Provider manages the infrastructure.

### Disadvantages

* Usually require an API key.
* Usage may incur costs.
* Cannot access or modify the model weights.
* Data is sent to the provider's servers according to their policies.

---

## Open Source vs Closed Source

| Open Source                      | Closed Source                                  |
| -------------------------------- | ---------------------------------------------- |
| Model weights are public.        | Model weights are private.                     |
| Can be fine-tuned.               | Cannot be fine-tuned by users (in most cases). |
| Can run locally.                 | Runs on the provider's servers.                |
| Better privacy when run locally. | Data is sent through the provider's API.       |
| Requires local hardware.         | Does not require powerful local hardware.      |

---

## What I Learned

* Open source models give more control and can be run on my own computer.
* Closed source models are accessed through APIs provided by companies.
* Open source models are suitable when customization and privacy are important.
* Closed source models are suitable when I want an easy-to-use, managed solution.

---

## Next Topic

Hugging Face and running open source models using LangChain.
