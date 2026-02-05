# 🏝️ Gemini AI Agent — End-to-End Full-Stack Implementation

This repository presents a **fully deployed, end-to-end AI Agent system** running on real cloud infrastructure.  
The project demonstrates how to design, orchestrate, and serve a modern **LLM-powered conversational agent** using a clean, modular architecture.

The system is deployed on **AWS EC2 (Ubuntu 24.04 LTS)** and integrates:

- **Google Gemini 1.5 Flash** as the core language model  
- **Flowise AI** as the agent orchestration and memory layer  
- **Node.js / Express** as the backend API gateway  
- A lightweight **HTML/CSS floating chat UI** for user interaction  

This project is intentionally built to resemble a **production-style AI service**, not a local demo or notebook experiment.

---

## 🔗 Live Demo

A live instance of the AI Agent is publicly available:

👉 **http://18.219.123.65:3000/**

The demo features a floating chat widget connected to a live Gemini-powered agent through Flowise.

---

## 🎯 Project Goals

- Deploy a real AI Agent on cloud infrastructure (AWS EC2)
- Separate **LLM logic**, **API layer**, and **frontend UI**
- Enable **memory-aware conversations**
- Use low-code AI tooling without hiding system architecture
- Provide a reproducible reference for AI agent deployment

---

## 🧠 System Architecture Overview

The system is composed of four clearly separated layers:

### Architectural Rationale

- **Frontend** remains stateless and lightweight  
- **Backend** acts as a secure gateway and abstraction layer  
- **Flowise** manages agent logic and memory without hardcoding  
- **LLM provider** can be swapped without UI changes  

This separation makes the system extensible, debuggable, and production-friendly.

---

## 🚀 Technology Stack

### Cloud & OS
- AWS EC2
- Ubuntu 24.04 LTS

### AI & Orchestration
- Google Gemini 1.5 Flash
- Flowise AI
  - Conversation chains
  - Memory nodes
  - API-based execution

### Backend
- Node.js (v20)
- Express.js
- Axios
- REST-based communication with Flowise

### Frontend
- HTML5 / CSS3
- Floating chat widget
- No frontend framework (intentionally minimal)
- Served as static assets via Node.js

---

### 📁 Project Structure

The project is organized with a clear separation between the backend server and the frontend assets.

```text
/home/ai-agent
├── app.js
├── package.json
└── public/
    ├── index.html
    ├── style.css
    └── script.js

