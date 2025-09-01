# Make.com: Agentic Email Reader & Summarizer

This repository contains the **blueprints and documentation** for a **full-stack, no-code agentic AI tool** that automates the processing of your email inbox.  

The system connects to your email account, automatically summarizes messages, classifies them by priority, and provides a simple user interface for quick, actionable responses.

---

## 📌 Executive Summary

The **Agentic Email Reader & Summarizer** is designed to save office workers time by automatically triaging their inbox.  

- Fetches unread emails  
- Uses an AI model to generate concise summaries  
- Assigns a priority level (**HIGH / MEDIUM / LOW**)  
- Stores the results in a database  
- Provides a streamlined dashboard for review and action  

---

## 🚀 Key Features

- **Automated Email Fetching** → Connects to Gmail or Microsoft 365 inbox.  
- **AI-Powered Summaries** → Generates 1–3 sentence summaries using an LLM (e.g., OpenAI).  
- **Priority Classification** → Deterministic rules + optional LLM verification.  
- **Centralized Data Storage** → Airtable stores summaries, metadata, and priorities.  
- **User Interface** → Dashboard (Retool/Bubble) for quick review and actions.  
- **Agentic Actions** → Sends Slack notifications for high-priority emails.  
- **Safety First** → No auto-sending; every step requires explicit approval and is logged.  

---

## 🏗️ High-Level Architecture

This project leverages **no-code/low-code tools** to orchestrate the workflow:

- **Email Connector** → Gmail or Microsoft 365 (Make.com trigger)  
- **Orchestration** → Make.com scenario to chain modules  
- **AI Engine** → Summarization & classification via LLM (OpenAI through HTTP module)  
- **Database** → Airtable for structured storage (summaries, actions, logs)  
- **Frontend UI** → Retool or Bubble dashboard connected to Airtable  
- **Notifications** → Slack integration for high-priority alerts  

---

## 🔑 Prerequisites

You will need accounts & API keys for:

- [Make.com](https://www.make.com/) – automation host  
- [Airtable](https://airtable.com/) – database  
- [OpenAI](https://platform.openai.com/) – AI summarization  
- Gmail / Microsoft 365 – email source  
- [Retool](https://retool.com/) / [Bubble](https://bubble.io/) – dashboard UI  
- Slack (optional) – notifications  

---
