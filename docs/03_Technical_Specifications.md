# Technical Specifications

## 9. Database Design (MySQL)
The database will be relational, managed via SQLAlchemy ORM.

**Tables:**
*   **`users`**: id, name, email, password_hash, role (student, faculty, admin).
*   **`locations`**: id, name, type (classroom, lab, cabin, amenity), building, floor, node_id (for navigation graph).
*   **`faculty`**: id, user_id, department, cabin_location_id, office_hours.
*   **`events`**: id, title, description, start_time, end_time, location_id.
*   **`graph_nodes`**: id, x_coord, y_coord, floor, building.
*   **`graph_edges`**: id, node_a_id, node_b_id, distance_weight.

## 10. API Design (FastAPI)
Base URL: `/api/v1`

**Authentication:**
*   `POST /auth/login` - Returns JWT token.
*   `POST /auth/register` - Creates a new user.

**AI & Chat:**
*   `POST /chat/ask` - Accepts `{"message": "..."}`, returns Gemini AI response.

**Navigation:**
*   `GET /nav/route?start={node_id}&end={node_id}` - Returns an array of coordinates forming the shortest path.
*   `GET /locations/search?q={query}` - Returns matching locations/rooms.

**Faculty & Events:**
*   `GET /faculty/search?name={name}` - Returns faculty details and cabin location.
*   `GET /events/upcoming` - Returns list of active events.

## 11. Frontend Architecture (React)
*   **State Management:** Zustand or Redux Toolkit for managing user sessions and active navigation routes.
*   **Routing:** React Router DOM (Pages: Home, Chat, Map, Directory, Notices).
*   **Map Rendering:** Leaflet.js or React-Map-GL for overlaying the path array onto an image/vector map of the campus.
*   **Styling:** Tailwind CSS for rapid, utility-first styling. Shadcn UI for accessible pre-built components (buttons, modals, inputs).

## 15. Folder Structure
```text
CampusConnectAI/
├── backend/                  # FastAPI Application
│   ├── app/
│   │   ├── api/              # Route handlers (chat, nav, auth)
│   │   ├── core/             # Config, security, Gemini setup
│   │   ├── db/               # SQLAlchemy models and migrations
│   │   ├── services/         # Business logic (A* algorithm, RAG)
│   │   └── main.py           # Application entry point
│   ├── requirements.txt
│   └── .env
├── frontend/                 # React Application
│   ├── src/
│   │   ├── components/       # Reusable UI (ChatBubble, MapOverlay)
│   │   ├── pages/            # View components (Home, Map, Chat)
│   │   ├── hooks/            # Custom React hooks (useMap, useChat)
│   │   ├── store/            # Zustand state
│   │   ├── App.jsx
│   │   └── index.css
│   ├── package.json
│   └── tailwind.config.js
└── README.md
```

## 16. GitHub Repository Structure
*   **`main` branch:** Production-ready code.
*   **`dev` branch:** Integration branch for testing.
*   **Feature branches:** `feat/ai-chat`, `feat/astar-nav`, `fix/login-bug`.
*   **`.github/workflows/`**: CI/CD pipelines (GitHub Actions) for running PyTest on backend and ESLint on frontend.
