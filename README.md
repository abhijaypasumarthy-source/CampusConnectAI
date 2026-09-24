<div align="center">
  <h1>🎓 CampusConnect AI 🤖</h1>
  <p><i>An AI-Powered Student Information & Smart Navigation Platform</i></p>
</div>

<br />

CampusConnect AI is a unified campus assistant designed to help students, faculty, and visitors seamlessly navigate university spaces, discover events, and find academic information instantly using a Generative AI conversational interface.

## 🌟 Key Features

*   **Intelligent AI Assistant:** Powered by the Gemini API. Ask natural language questions ("Where is AB1-304?", "When is the tech fest?") and receive context-aware answers.
*   **Smart Campus Navigation:** Computes the shortest paths between buildings, departments, and specific rooms using A* graphing algorithms.
*   **Faculty Directory:** Instantly search for professors, view their office hours, and get routing to their cabins.
*   **Event & Notice Hub:** Centralized digital bulletin board for campus announcements.

## 📚 Documentation

The complete architectural blueprint and project plan are available in the [`docs/`](./docs) directory:

1. [**Product Strategy & Requirements**](./docs/01_Product_Strategy_and_Requirements.md) (Vision, Target Users, Feature List)
2. [**System Architecture & Design**](./docs/02_System_Architecture_and_Design.md) (RAG AI Design, Navigation Engine, Flow Diagrams)
3. [**Technical Specifications**](./docs/03_Technical_Specifications.md) (Database Schema, API Design, Repository Structure)
4. [**UI/UX Wireframes**](./docs/04_UI_UX_Wireframes.md) (Layouts for Chat, Dashboard, and Map Navigation)
5. [**Project Roadmap**](./docs/05_Project_Roadmap.md) (MVP definition, Development Phases)

## 🛠️ Tech Stack

*   **Frontend:** React, Tailwind CSS, Leaflet.js
*   **Backend:** Python, FastAPI
*   **Database:** MySQL, SQLAlchemy ORM
*   **AI Engine:** Google Gemini API (RAG Architecture)

## 🏗️ Architecture Overview

The system utilizes a **Retrieval-Augmented Generation (RAG)** approach. When a user asks a question, the FastAPI backend intercepts the query, retrieves factual campus data (room coordinates, faculty info) from the MySQL database, and injects this context into the Gemini API prompt. This ensures the AI provides accurate, hallucination-free answers specific to your university.

## 🚀 Roadmap

*   [x] Project Planning & System Architecture
*   [ ] Database Schema & Backend Boilerplate
*   [ ] Gemini API RAG Integration
*   [ ] A* Navigation Algorithm Implementation
*   [ ] React Frontend & UI Wiring

## 📝 License

This project design is in the planning and development phase.
