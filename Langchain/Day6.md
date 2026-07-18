# Day 5 - Temperature and Prompts

## 📅 Date

16 July 2026

## Temperature

Temperature controls the **randomness** of the model's output.

### Temperature = 0

* Gives **consistent and predictable** responses.
* Same prompt → almost same output every time.
* Best for **code generation, math, and factual tasks**.

**Why?**
The model assigns probabilities to possible next tokens (words). At temperature 0, it almost always chooses the token with the **highest probability**, so the output becomes nearly deterministic.

### Temperature = 0.5 - 0.7

* Balanced between consistency and creativity.
* Good for **chatbots and general conversations**.

### Temperature = 0.8 - 1.0

* More random and creative.
* Good for **story writing, brainstorming, and creative content**.

---

## Prompts

A **prompt** is the input or instruction given to a language model.

### Static Prompt

* Prompt is hardcoded in the code.
* To change the question, the developer must modify the code.

Example:

```python
model.invoke("What is AI?")
```

### Dynamic Prompt

* Prompt is taken from user input or a variable.
* The code remains the same; only the input changes.

Example:

```python
question = input("Ask a question: ")
model.invoke(question)
```

---

## What I Learned

* Temperature controls output randomness.
* Lower temperature → more consistent responses.
* Higher temperature → more creative responses.
* Prompts are the instructions given to a model.
* Static prompts require code changes.
* Dynamic prompts allow different inputs without changing the code.
