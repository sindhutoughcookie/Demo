# 🏨 AI Hotel Assistant Demo (AI Architecture)

## 📌 Overview

This project demonstrates how to build a **production-inspired AI system** using a simple *hotel assistant* use case.

The notebook showcases how modern AI applications combine:
- Prompt orchestration  
- Retrieval-Augmented Generation (RAG)  
- Guardrails (input/output safety)  
- LLM API interaction  

This is designed as a **teaching/demo artifact** to illustrate core AI system architecture concepts.

---

## 🚀 How to Run

1. Open the workspace link [demo](https://curly-space-journey-5gjwr4wg4ppph45j9.github.dev/)  
2. Create a .env file in the workspace root:
  - OPENAI_API_KEY=your-api-key
  - AZURE_OPENAI_ENDPOINT=your-endpoint
3. Create or open the notebook file: hotel_demo.ipynb
4. Run each block

## 🧩 System Design Choices

This demo is intentionally designed to reflect how real-world AI systems are built, while keeping the implementation simple and teachable. Below are the key system design decisions and the reasoning behind them.


| Design Choice | Reason |
|--------------|--------|
| GPT-4o mini | Balance of quality, cost, latency |
| Prompting over fine-tuning | Faster iteration, simpler |
| RAG | In memory for demo simplicity. Replaceable with vector DB (e.g., Azure AI Search) for efficient large-scale retrieval  |
| Temperature 0.3 | Deterministic, predictable, consistent |
| Managed Model Scaling (Azure) | Automatically handles scaling, availability, and infrastructure for model inference |
| Backend scaling | Not relavent for demo


