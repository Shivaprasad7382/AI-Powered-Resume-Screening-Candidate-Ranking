AI-Powered Resume Screening & Candidate Ranking

> NLP-based resume screening system using TF-IDF cosine similarity to rank candidates against job descriptions and identify skill gaps.

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-3.0-000000?style=for-the-badge&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-10b981?style=for-the-badge)

---

## ✨ Features

- **TF-IDF cosine similarity for resume-to-job matching** — TF-IDF cosine similarity for resume-to-job matching
- **Skill gap analysis** — matched vs missing skills
- **Experience-based scoring** — Experience-based scoring
- **Auto-shortlisting of top 3 candidates per job** — Auto-shortlisting of top 3 candidates per job
- **Candidate ranking with explainable scores** — Candidate ranking with explainable scores

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | Python 3.10+, Flask 3.x |
| Database | MySQL 8.x, mysql-connector-python |
| ML / NLP | Scikit-learn, Pandas, NumPy |
| Frontend | HTML5, CSS3, Chart.js, Jinja2 |

---

## 📁 Project Structure

```
resume-screening/
├── app.py              ← Flask application + API routes
├── schema.sql          ← Database schema + seed data
├── requirements.txt    ← Python dependencies
├── .gitignore
├── LICENSE
└── templates/
    └── dashboard.html  ← Interactive dashboard UI
```

---

## ⚙️ Setup & Installation

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/resume-screening.git
cd resume-screening
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Configure database
Edit `DB_CONFIG` in `app.py`:
```python
DB_CONFIG = {
    "host":     "localhost",
    "user":     "your_mysql_user",
    "password": "your_mysql_password",
    "database": "resume_db"
}
```

### 4. Initialize the database
```bash
mysql -u root -p < schema.sql
```

### 5. Run the application
```bash
python app.py
```

Visit: **[http://localhost:5011](http://localhost:5011)**

---

## 🗄️ Database Tables

```
job_postings, candidates, applications
```

---

## 🚀 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Main dashboard |
| GET/POST | `/api/*` | REST API endpoints |


