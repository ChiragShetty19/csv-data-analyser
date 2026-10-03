# 📊 DataLens — CSV Data Analyzer & AI Insights

[![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/React_19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

> A modern, full-stack web application designed to instantly analyze, visualize, and extract intelligent insights from CSV datasets with zero configuration.

---

## ✨ Features

- **⚡ Instant File Upload & Processing**: Fast drag-and-drop CSV ingestion with automatic parsing and schema detection.
- **📈 Comprehensive Statistical Analysis**: Computes shape, column types, count, mean, min, max, standard deviation, and categorical frequencies.
- **🔍 Data Quality & Health Check**: Highlights missing value rates and duplicate rows to identify cleaning requirements upfront.
- **📊 Interactive Data Visualizations**: Dynamic charts including Bar charts, Line charts, Pie charts, and Histograms powered by Recharts.
- **🤖 AI-Powered Insights**: Automated summary breakdown and intelligent findings generated via Google Gemini 3.8 Flash.
- **🎨 Sleek & Responsive UI**: Clean modern design built with React 19, Tailwind CSS, and Lucide icons.

---

## 🏗️ Architecture & Project Structure

```text
csv-data-analyzer/
├── datalens/
│   ├── backend/
│   │   ├── main.py              # FastAPI endpoints & CORS configuration
│   │   ├── analyzer.py          # Pandas statistical analysis & metrics engine
│   │   ├── ai_service.py        # Gemini API integration for automated insights
│   │   ├── requirements.txt     # Python dependencies
│   │   └── .env.example         # Template for environment variables
│   ├── frontend/
│   │   ├── src/
│   │   │   ├── components/      # Modular UI components (Charts, Tables, Upload)
│   │   │   ├── pages/           # Landing page & Analyzer dashboard
│   │   │   ├── App.jsx          # Router & application root
│   │   │   └── index.css        # Tailwind styling & theme
│   │   ├── package.json         # Frontend dependencies and scripts
│   │   └── vite.config.js       # Vite build setup
│   └── test_data.csv            # Sample dataset for quick evaluation
├── .gitignore                   # Ignores venv, node_modules, and secrets
├── LICENSE                      # MIT License
└── README.md                    # Project documentation
```

---

## 🚀 Quick Start Guide

### Prerequisites
- **Python 3.10+**
- **Node.js 18+** & npm

---

### 1. Backend Setup

1. Open a terminal and navigate to the backend directory:
   ```bash
   cd datalens/backend
   ```

2. Create and activate a virtual environment:
   ```bash
   # Windows (PowerShell)
   python -m venv venv
   .\venv\Scripts\Activate.ps1

   # Linux / macOS
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Configure environment variables (optional for AI insights):
   ```bash
   cp .env.example .env
   ```
   Add your [Google AI Studio API key](https://aistudio.google.com/):
   ```env
   GEMINI_API_KEY=your_gemini_api_key_here
   ```

5. Launch the FastAPI backend server:
   ```bash
   uvicorn main:app --reload
   ```
   *The API will be available at `http://localhost:8000` (docs at `http://localhost:8000/docs`).*

---

### 2. Frontend Setup

1. In a new terminal window, navigate to the frontend directory:
   ```bash
   cd datalens/frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the Vite development server:
   ```bash
   npm run dev
   ```
   *The frontend dashboard will run at `http://localhost:5173`.*

---

## 🧪 Testing with Sample Data

You can find a ready-to-use sample dataset at [`datalens/test_data.csv`](datalens/test_data.csv). Drag and drop this file directly onto the dashboard to preview analysis and generate charts instantly!

---

## 👤 Author

Developed by **[Chirag Shetty](https://github.com/ChiragShetty19)**

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
