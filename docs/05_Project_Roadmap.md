# Project Roadmap

## 17. Development Roadmap
*   **Phase 1: Foundation (Weeks 1-2)**
    *   Setup Git, DB schema, and FastAPI boilerplate.
    *   Design basic React frontend layout.
*   **Phase 2: Data & AI (Weeks 3-4)**
    *   Populate MySQL with dummy campus data (rooms, faculty).
    *   Integrate Gemini API and build RAG logic.
*   **Phase 3: Navigation Engine (Weeks 5-6)**
    *   Plot graph nodes for a section of the campus.
    *   Implement A* algorithm and map UI in React.
*   **Phase 4: Integration & Testing (Weeks 7-8)**
    *   Connect AI outputs to Navigation (Action Chips).
    *   User acceptance testing and bug fixing.

## 18. MVP Version (Minimum Viable Product)
The MVP will focus strictly on the most critical pain points:
1.  **AI Chatbot** capable of answering hardcoded database queries (faculty locations, basic campus info).
2.  **Basic Search Interface** for finding rooms.
3.  **Static Routing:** Text-based step-by-step directions without the complex interactive map rendering.

## 19. Future Enhancements
*   **AR Navigation:** Use WebXR/mobile camera for augmented reality arrows pointing to destinations.
*   **Live Location Tracking:** Integration with campus Wi-Fi to auto-detect "Current Location".
*   **Voice Integration:** Whisper API for speaking to the assistant.
*   **Timetable Sync:** Sync student Google Calendars to automatically suggest routes to the next class.
