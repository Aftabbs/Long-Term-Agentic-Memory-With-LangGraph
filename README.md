# 🧠 Long-Term Agentic Memory with LangGraph

![image](https://github.com/user-attachments/assets/669c0a9a-391e-49bf-9fe2-a71f7dc4f6b0)

This project explores the integration and evaluation of **semantic**, **episodic**, and **procedural memory** in autonomous agents using the LangGraph framework. We begin with a baseline email-handling agent and progressively enhance it with structured memory components to assess their impact on agent performance and decision-making.


![image](https://github.com/user-attachments/assets/56d8c780-4890-4751-86a2-381cfccad518)


![image](https://github.com/user-attachments/assets/559b029a-1c7c-442e-825d-aee672fbfded)

---

## 📌 Project Objective

To **experimentally validate** how various memory types—semantic, episodic, and procedural—affect the behavior and efficiency of an autonomous agent. We aim to simulate cognitive architectures for memory modeling in AI, specifically within the context of a **long-term memory-enabled email assistant**.

---

![image](https://github.com/user-attachments/assets/e3c26924-8cef-420d-aa94-49aa69287d5b)

![image](https://github.com/user-attachments/assets/672a9737-49f2-49f1-b40e-4f91c5648c7f)

![image](https://github.com/user-attachments/assets/9e720d38-1304-46d9-85db-de3bf0ffdd37)




## 🧱 Memory Architecture

1. **Semantic Memory**
   Stores structured knowledge (facts, concepts, context-free data).
   → Example: "John is a client from NY."

2. **Episodic Memory**
   Logs past experiences or interactions, time-stamped and context-bound.
   → Example: "John emailed about a billing issue on 2024-05-22."

3. **Procedural Memory**
   Encodes *how to do* things—agent's skills, routines, and task workflows.
   → Example: "When encountering a billing issue, forward to [finance@company.com](mailto:finance@company.com)."

---

## 🧪 Experimental Setup

We started with a **baseline email agent** performing actions like reading, summarizing, and responding to emails. Memory layers were added incrementally to this base agent:

* **Baseline**: No memory
* **+ Semantic Memory**
* **+ Semantic + Episodic Memory**
* **+ Semantic + Episodic + Procedural Memory**

---

##  Tech Stack

| Component             | Version |
| --------------------- | ------- |
| `langchain`           | 0.3.18  |
| `langgraph`           | 0.2.72  |
| `langmem`             | 0.0.8   |
| `langchain-openai`    | 0.3.5   |
| `langchain-anthropic` | 0.3.7   |

Used LangGraph for agentic flow construction, LangChain for LLM integration, and LangMem for custom memory backends.

---

## 📈 Evaluation

Each version of the agent was evaluated based on:

* **Memory Recall**: Accuracy of information retrieval
* **Context Awareness**: Ability to use memory for relevant actions
* **Task Completion Time**: Speed and efficiency
* **Interaction Coherence**: Smoothness and correctness of conversations

---

##  Key Learnings

* **Semantic memory** enhanced fact-based decision making.
* **Episodic memory** improved context retention over multiple turns.
* **Procedural memory** enabled learned routines for faster execution and reduced error.
* The layered memory approach reflects real-world cognitive systems and offers modular flexibility.

---

##  Future Work

* Fine-tuning memory decay and retrieval strategies.
* Multi-agent memory sharing.
* Integration with vector databases for large-scale semantic memory.



