
# 🗳️ Voter Turnout Analyzer

A full-stack application for large-scale voter data analysis using FastAPI (backend), Streamlit (frontend), and Fly.io (cloud hosting). This project enables the upload and intelligent analysis of voter registration and turnout data with support for massive datasets and AI-enhanced suggestions.

---

## 🔧 Features

- Upload and analyze large CSV files (up to 500MB)
- Intelligent column detection (precinct, vote method, totals, party, etc.)
- Precinct-level performance analysis and benchmarking
- Party registration and turnout breakdowns
- Voting method comparisons
- Registration efficiency and turnout funneling
- AI-powered civic engagement strategy suggestions (Claude/OpenAI)
- Export options: JSON, CSV, Markdown reports
- Hosted backend on Fly.io

---

## 🚀 Tech Stack

- **Backend**: FastAPI + Uvicorn
- **Frontend**: Streamlit + Plotly
- **AI Integration**: OpenAI / Anthropic API (Claude)
- **Hosting**: Fly.io
- **Data**: Pandas, NumPy

---

## 🧠 AI Key Setup (Optional)

- Create a `.env` file and include:
  ```
  OPENAI_API_KEY=your_openai_key
  ANTHROPIC_API_KEY=your_claude_key
  ```

---

## 📦 Installation (Local)

```bash
# 1. Clone this repo
git clone https://github.com/YOUR_USERNAME/voter-turnout-analyzer.git
cd voter-turnout-analyzer

# 2. Setup backend
cd backend
pip install -r requirements.txt
uvicorn main:app --reload

# 3. Setup frontend
cd ../frontend
pip install -r requirements.txt
streamlit run streamlit_app.py
```

---

## ☁️ Deployment on Fly.io

```bash
flyctl launch  # follow prompts
flyctl deploy
```

---

## 📂 Folder Structure

```
voter-turnout-enhanced/
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   ├── Dockerfile
│   └── fly.toml
├── frontend/
│   ├── streamlit_app.py
│   └── requirements.txt
└── docs/
    └── README.md
```

---

## ✅ To-Do

- Add user authentication via OAuth (optional)
- Improve AI strategy templating
- Setup CI/CD with GitHub Actions
