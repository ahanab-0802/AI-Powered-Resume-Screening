## AI Resume Screener & Job Matcher

An AI-powered Resume Screening and Job Matching system developed for the **Cognizant NPN AIA Hackathon**. It analyzes resumes against Job Descriptions, calculates an explainable match score, identifies matched/missing skills, measures semantic similarity, and generates personalized recommendations.

## 🚀 Live Demo

**AWS EC2:** http://43.204.237.177:8501/

## 🔄 Workflow

```text
Resume + Job Description
          ↓
     AI Analysis
          ↓
     Match Score
          ↓
Matched & Missing Skills
          ↓
 Recommendations
          ↓
      PDF Report
```

## ⚙️ Environment Configuration

Create a `.env` file in the project root:

```env
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key

GROQ_API_KEY=your_groq_api_key
GROQ_MODEL=openai/gpt-oss-120b

HF_TOKEN=your_huggingface_token
```

**Never commit `.env` or expose API keys.**

Add to `.gitignore`:

```gitignore
.env
venv/
__pycache__/
```

## 🛠️ Setup

```bash
git clone https://github.com/YOUR_USERNAME/AI-Resume-Screening-ATS.git
cd AI-Resume-Screening-ATS

python -m venv venv
pip install -r requirements.txt
```

Start backend:

```bash
python -m uvicorn backend.main:app --reload
```

Start frontend:

```bash
python -m streamlit run frontend/streamlit_app.py
```

* Backend: `http://127.0.0.1:8000`
* API Docs: `http://127.0.0.1:8000/docs`
* Frontend: `http://localhost:8501`

## 🧰 Tech Stack

**Frontend:** Streamlit, HTML/CSS
**Backend:** Python, FastAPI, Uvicorn
**AI/NLP:** spaCy, Sentence Transformers, all-MiniLM-L6-v2, Groq
**ML:** Scikit-learn, NumPy, Pandas
**Database:** Supabase, PostgreSQL
**PDF:** WeasyPrint
**Deployment:** AWS EC2

## 👩‍💻 Contribution

Developed collaboratively for the **Cognizant NPN AIA Hackathon**.

My primary contributions included **ATS scoring, semantic similarity, skill matching and validation, missing-skill identification, AI feedback generation, and backend integration**.
