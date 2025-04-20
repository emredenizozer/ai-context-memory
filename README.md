## Large Language Models: With and Without Memory

This repository provides two Python examples demonstrating the difference in behavior between large language models (LLMs) **with memory** and **without memory**. It highlights a key characteristic of most current LLMs: **they do not retain information across interactions unless explicitly designed to do so.**

## 📌 Key Concept

By default, LLMs **do not have memory** — they do not retain or store past conversations. Every message is processed in isolation or within the immediate context window. This has important implications for how you design and interact with such systems.

In contrast, when **memory is implemented**, the model is able to recall previous inputs, maintain ongoing context, and deliver more coherent, context-aware responses over longer conversations or sessions.

---

## 📁 Files

### 1. `no_memory.py`

- Simulates an LLM without memory.
- Each message is treated as a standalone input.
- Demonstrates how the model fails to recall prior context or user preferences.

### 2. `ctx_memory.py`

- Simulates an LLM with memory.
- Stores conversation history or user data across turns.
- Demonstrates how past interactions influence future responses, allowing for more personalized and coherent output.

---

## 🚀 How to Run

### 1. Install Dependencies

Make sure you have Python 3 installed. Install required packages using:

```bash
pip install -r requirements.txt
```

### 2. Set Up Your .env File
Create a .env file in the root of the project with your OpenAI API key:

```bash
OPENAI_API_KEY=your-openai-api-key-here
```
⚠️ This file is automatically used by the script to authenticate with OpenAI.

### 3. Run the Script

```bash
python3 no_memory.py
python3 ctx_memory.py
```

### 4. Interact With the Assistant

Once running, you can choose which model to use:

- 1 → OpenAI GPT-4

- 2 → Ollama (local model)
  <br /><br />
  
Then start chatting. Available commands:

- save – Save the conversation to conversation.json

- load – Load the conversation from file

- summary – Summarize recent conversation to save tokens

- quit – Exit the program



