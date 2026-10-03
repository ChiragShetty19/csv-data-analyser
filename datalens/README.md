# DataLens - CSV Data Analyzer

A simple, modern web application to upload a CSV file and quickly understand the dataset through statistics, charts, and simple AI-generated insights.

## Features
- CSV Upload (drag & drop)
- Dataset summary & column metadata
- Missing values analysis
- Interactive charts (Bar, Line, Pie, Histogram)
- AI-generated insights (powered by Google Gemini)

## Tech Stack
- **Frontend:** React 19, Vite, Tailwind CSS, Recharts, Lucide Icons
- **Backend:** FastAPI, Pandas, Google GenAI SDK (`gemini-3.8-flash`), Python-multipart, Uvicorn

## Setup Instructions

### 1. Backend
Navigate to the backend directory:
```bash
cd backend
```

Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

Install dependencies:
```bash
pip install -r requirements.txt
```

Set up environment variables:
Create a `.env` file from `.env.example` and add your Google Gemini API key (optional for AI insights):
```bash
GEMINI_API_KEY=your_gemini_api_key
```

Run the FastAPI server:
```bash
uvicorn main:app --reload
```
The backend API runs at `http://localhost:8000`.

### 2. Frontend
Navigate to the frontend directory:
```bash
cd frontend
```

Install dependencies:
```bash
npm install
```

Run the development server:
```bash
npm run dev
```

Open your browser at `http://localhost:5173`.
