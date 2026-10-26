
# AI Retail Analytics Platform

## Phase 2: Inventory Analytics Dashboard Complete 🎉

## Folder Structure
```
AI Retail/
├── backend/
│   ├── ai_retail/
│   │   ├── __init__.py
│   │   ├── settings.py
│   │   ├── urls.py
│   │   ├── wsgi.py
│   │   └── asgi.py
│   ├── new_venv/ (virtual environment)
│   ├── manage.py
│   ├── requirements.txt
│   ├── .env
│   └── .env.example
└── frontend/
    ├── src/
    │   ├── components/
    │   │   ├── Sidebar.tsx
    │   │   └── StatsCard.tsx
    │   ├── lib/
    │   ├── pages/
    │   │   └── Home.tsx
    │   ├── App.tsx
    │   ├── main.tsx
    │   └── index.css
    ├── index.html
    ├── vite.config.ts
    ├── tsconfig.json
    ├── tsconfig.node.json
    ├── tailwind.config.js
    ├── postcss.config.js
    ├── package.json
    └── .env.example
```

## What's New in Phase 2
✅ Sidebar navigation with menu items
✅ Statistics cards with trend indicators
✅ Inventory bar chart using Recharts
✅ Professional, responsive dashboard layout

---

## How to Run in VS Code (Step by Step)

### Prerequisites
- Install Python (3.10+) from https://www.python.org/
- Install Node.js (18+) from https://nodejs.org/

---

## 1. Backend Setup (Terminal 1)
Open **New Terminal** in VS Code:
```bash
# Navigate to backend directory
cd backend

# Create & activate virtual environment (only first time)
python -m venv new_venv
.\new_venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run initial database migrations
python manage.py migrate

# Start backend server
python manage.py runserver
```
Backend will be available at: **http://localhost:8000**

---

## 2. Frontend Setup (Terminal 2)
Open **New Terminal** in VS Code (split terminal):
```bash
# Navigate to frontend directory
cd frontend

# Install dependencies (only first time)
npm install

# Start frontend dev server
npm run dev
```
Frontend will be available at: **http://localhost:5173** (open this in your browser!)

---

## Common Errors and Fixes
- "Django not found": Make sure you activated the virtual environment (.\new_venv\Scripts\activate)
- "npm not found": Ensure Node.js is installed and added to your system PATH
- Seeing directory listing at 127.0.0.1:5500: You're using VS Code Live Server—stop it and use `npm run dev` in frontend folder instead!

## Expected Output
- Frontend: You'll see the full inventory analytics dashboard with sidebar, stats cards, and chart!
- Backend: You'll see the Django default page at http://localhost:8000

## Next Phase (After Confirmation)
We'll connect the frontend to a real Django backend API with actual inventory data!
