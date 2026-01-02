#  Saree Inventory AI Chatbot

[![n8n](https://img.shields.io/badge/Workflow-n8n-FF6D5A?style=flat&logo=n8n&logoColor=white)](https://n8n.io/)
[![Google Gemini](https://img.shields.io/badge/AI-Google%20Gemini-4285F4?style=flat&logo=google-gemini&logoColor=white)](https://deepmind.google/technologies/gemini/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An intelligent, web-based conversational assistant that allows users to query a saree inventory in natural language. By bridging a modern frontend with **n8n** and **Google Gemini**, this project turns a static Excel sheet into a smart retail assistant.

---

##  Project Architecture



The system follows a modular flow to ensure low latency and high accuracy:
1. **Frontend:** User interaction via a clean HTML/JS interface.
2. **Orchestration:** n8n acts as the "brain," managing data flow and webhooks.
3. **Data Layer:** Excel serves as the lightweight database for stock management.
4. **Intelligence:** Google Gemini processes natural language and generates human-like responses.

---

##  Key Features

- **Natural Language Inventory Queries**  
  Ask conversational questions like *“Show silk sarees under ₹5,000”* or *“Which wedding sarees are available in red?”* without relying on rigid filters.

- **Real-Time Inventory Synchronization**  
  Inventory is read directly from an Excel source—any update to the file is reflected instantly without restarting the system.

- **AI-Powered Intent Understanding**  
  Leverages a Large Language Model (Google Gemini) to interpret user intent, handle ambiguous queries, and generate human-like responses grounded in structured data.

- **Visual Workflow Automation (Low-Code Backend)**  
  Uses n8n’s node-based workflows to manage data ingestion, business logic, and AI orchestration—no hard-coded backend required.

- **Non-Blocking, Asynchronous Frontend**  
  Fetch API–based communication ensures the UI remains responsive while AI processing happens in the background.

- **Modular & Extensible Architecture**  
  Each layer (UI, workflow, data, AI) is loosely coupled, making it easy to swap Excel for a database or add new features.

- **Production-Inspired Design**  
  Mimics real-world retail systems by separating data, logic, and AI reasoning—ideal for scaling and future enhancements.

- **Beginner-Friendly & Customizable**  
  Designed to be easily understood, modified, and extended by students or developers exploring automation and AI integration.


---

##  Tech Stack

| Component | Technology |
| :--- | :--- |
| **Frontend** | HTML5, CSS3, Vanilla JavaScript |
| **Backend Automation** | [n8n](https://n8n.io/) |
| **AI Model** | Google Gemini (LLM) |
| **Data Storage** | Excel (.xlsx / .csv) |



##  Project Structure

```bash
saree-chatbot/
├── frontend/
│   ├── index.html       # Chat UI & JS logic
│   └── styles.css       # Custom styling
├── n8n/
│   └── workflow.json    # Exported n8n workflow
├── data/
│   └── inventory.xlsx   # Sample Saree data
└── README.md

