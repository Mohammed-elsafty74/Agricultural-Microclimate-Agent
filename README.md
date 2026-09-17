# 🌱 Agricultural Microclimate Agent

An AI-powered agricultural decision-support system that analyzes environmental conditions and crop-specific agronomic knowledge to provide explainable microclimate risk assessments and actionable field recommendations.

Built for the **FortyGuard Hackathon '26**.

---

## 🚀 Overview

The **Agricultural Microclimate Agent** combines real-time environmental data, satellite climate information, and **RAG-based agricultural knowledge** to help farmers and agronomists understand heat and moisture-related risks affecting crops.

The system uses an **agentic architecture** that dynamically selects the required tools, retrieves relevant crop-specific evidence, evaluates environmental conditions, and generates grounded recommendations.

### Supported Crops

* 🍅 Tomato
* 🌰 Almond
* 🌽 Corn
* 🍇 Grape
* 🌱 Cotton

---

## 🧠 AI & RAG Architecture

The system is built around three main layers:

### Environmental Data Fusion

Combines multiple sources to build a field-level environmental profile:

* **FortyGuard** — Thermal surface data and heat statistics
* **NASA POWER** — Precipitation, soil moisture, and humidity data
* **US Census Geocoder** — Location and coordinate resolution

### 🌾 Grounded RAG Knowledge System

A crop-specific knowledge base built from agricultural extension publications.

* Vector-based document retrieval
* Crop-specific retrieval filtering
* Evidence-based recommendations
* Citation traceability
* Protection against cross-crop knowledge leakage

### 🤖 Agentic Decision Engine

An autonomous orchestration layer that:

1. Parses the user's agricultural goal.
2. Identifies the required data sources.
3. Dynamically selects the appropriate tools.
4. Retrieves relevant agronomic evidence.
5. Compares environmental observations with crop-specific thresholds.
6. Produces an explainable risk assessment.
7. Generates actionable recommendations.
8. Provides an execution trace for transparency.

If the available evidence is insufficient, the system returns **`INSUFFICIENT_EVIDENCE`** instead of generating unsupported conclusions.

---

## 🖥️ Web Dashboard

The project includes a modern agricultural dashboard built with **React + Vite**, providing:

* 📍 Interactive field location selection
* 🌱 Crop and growth-stage selection
* 📊 Environmental metrics
* 🌡️ Heat-risk assessment
* 📚 Evidence and source references
* 💡 Recommended field actions
* 🤖 Agent execution trace

The decision workflow is organized into:

**Field Location → Crop & Stage → Goal → Analysis → Decision Report**

---

## 🛠️ Tech Stack

| Category   | Technologies                         |
| ---------- | ------------------------------------ |
| AI / ML    | Python, Machine Learning             |
| RAG        | Vector Retrieval, Knowledge Base     |
| Agent      | Agentic Workflow, Tool Orchestration |
| Backend    | FastAPI                              |
| Frontend   | React, Vite                          |
| Data       | FortyGuard, NASA POWER               |
| Geospatial | Leaflet, US Census Geocoder          |
| Testing    | Python Unit & Integration Tests      |

---

## 🧪 Testing

The system includes automated tests covering:

* Agent orchestration
* RAG retrieval
* Crop scope validation
* Geocoding
* NASA POWER integration
* FortyGuard services

**45/45 tests passing** across the complete test suite.

---

## 🏗️ Architecture

```text
User Query
    │
    ▼
Goal Parser
    │
    ▼
Dynamic Agent Planner
    │
    ├──────────────► Geocoding
    │
    ├──────────────► FortyGuard Thermal Data
    │
    ├──────────────► NASA POWER
    │
    └──────────────► Crop-Specific RAG
                          │
                          ▼
                   Evidence & Thresholds
                          │
                          ▼
                   Decision Engine
                          │
                          ▼
              Risk Assessment + Actions
                          │
                          ▼
                   Web Dashboard
```

---

## 🎯 Key Highlights

* **Agentic AI** for dynamic decision-making
* **RAG** for grounded agricultural knowledge
* **Multi-source environmental data fusion**
* **Crop-specific evidence retrieval**
* **Explainable risk assessment**
* **Citation-backed recommendations**
* **Insufficient-evidence protection**
* **Full agent execution tracing**
* **Interactive agricultural dashboard**

---

## 🏆 Hackathon Project

Developed for the **FortyGuard Hackathon '26**, focusing on applying AI agents, RAG, environmental intelligence, and modern web technologies to agricultural decision support.

---

### 👨‍💻 Project Focus

**Artificial Intelligence · RAG · AI Agents · Environmental Data · Agriculture · Decision Support**
