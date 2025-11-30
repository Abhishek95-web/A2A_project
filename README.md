# 🏋️‍♂️ AI Fitness Assistant — Multi-Agent System with Gemini ADK

This project implements a lightweight but complete **multi-agent fitness assistant** using Gemini 2.5 Flash Lite and the **Google Agents Development Kit (ADK)**.

The system demonstrates:
- Agent-to-Agent (A2A) communication  
- Custom tool integration  
- Multi-agent orchestration  
- Session handling with Runner + InMemorySessionService  
- Structured personas and context engineering  
- Clean modular agent architecture  

It was built as part of the **AI Agents Intensive Capstone Project** on Kaggle.

---

## 🚀 Overview

The project has two core agents:

### **1. Exercise Catalog Agent**
A specialist agent responsible for retrieving factual exercise information.  
It uses a custom tool `get_exercise_info()` that contains structured details like:
- Muscles targeted  
- Difficulty level  
- Equipment needed  
- Reps or duration  

### **2. User Agent**
A front-facing concierge-style fitness assistant.  
It receives user queries and **delegates them** to the Exercise Catalog Agent through **A2A communication**, then returns a friendly, helpful explanation.

This demonstrates clean separation of responsibilities:
- User Agent → conversation, explanation  
- Exercise Agent → factual lookup  
- Tool → deterministic data source  

---

## 🔄 Architecture Diagram




---

## 🧠 Why This Project?

Beginners often struggle to understand exercises properly—muscles, difficulty, equipment, reps, etc.  
This project solves that by building a small AI assistant that:
- Understands the user’s request  
- Delegates the query to an expert agent  
- Fetches accurate exercise data via a tool  
- Returns a friendly, structured response  

---

## 📦 Tech Stack

- **Gemini 2.5 Flash Lite**
- **Google Agents Development Kit**
- **LlmAgent**
- **InMemorySessionService**
- **Runner & run_async()**
- **Custom Python tools**

---

## 🧪 Demo

Run the A2A test:

```python
await test_a2a_communication("Tell me about Push Ups. What muscles do they work?")
```



## 💬 Acknowledgements
This project was built as part of the Kaggle AI Agents Intensive using the Google Agents Development Kit (ADK) and Gemini models. Special thanks to the Kaggle team and Google DeepMind for the course resources and guidance.



