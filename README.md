# 📄 AI Resume Screening Agent

An AI-powered Resume Screening Agent built with **n8n** that automatically extracts information from PDF resumes, analyzes candidate profiles using AI, compares them with job requirements, calculates a match score, stores results in Google Sheets, and returns structured JSON responses.

---

## 🚀 Features

- 📄 Upload PDF resumes through a Webhook
- 📝 Extract text from PDF resumes
- 🤖 AI-powered resume analysis
- 📊 ATS-style candidate scoring
- 🎯 Compare resume against job description
- ✅ Identify matching and missing skills
- 📧 Extract candidate details
  - Name
  - Email
  - Phone Number
- 📈 Generate hiring recommendations
- 📑 Store screening results in Google Sheets
- 🔗 Return structured JSON via API

---

## 🏗 Workflow Architecture

```text
Webhook
   │
   ▼
Extract Resume Text
   │
   ▼
AI Resume Analyzer
   │
   ▼
JSON Parser
   │
   ▼
Google Sheets
   │
   ▼
Respond to Webhook
```

---

## 🛠 Technologies Used

- n8n
- Groq API (Llama 3.3)
- Google Sheets
- Webhook API
- JavaScript (Code Node)
- AI Agent
- Extract From File Node

---

## 📂 Project Structure

```
AI-Resume-Screening-Agent/
│
├── README.md
├── AI Resume Screening Agent.json
├── screenshots/
│   ├── workflow.png
│   ├── webhook-response.png
│   └── google-sheet.png
└── LICENSE
```

---

## ⚙️ How It Works

1. User uploads a PDF resume.
2. The workflow extracts the text from the PDF.
3. AI analyzes the resume.
4. Candidate details are extracted.
5. Resume is compared with the job description.
6. Match score is calculated.
7. Recommendation is generated.
8. Results are stored in Google Sheets.
9. API returns structured JSON.

---

## 📥 Installation

1. Clone the repository.

```bash
git clone https://github.com/YOUR_USERNAME/AI-Resume-Screening-Agent.git
```

2. Open n8n.

3. Import:

```
AI Resume Screening Agent.json
```

4. Configure credentials:

- Groq API
- Google Sheets OAuth

5. Execute the workflow.

---

## 📤 Example API Response

```json
{
  "candidate_name": "John Doe",
  "email": "john@example.com",
  "phone": "+1 9876543210",
  "match_score": 87,
  "matching_skills": [
    "React",
    "Node.js",
    "MongoDB"
  ],
  "missing_skills": [
    "Docker",
    "AWS"
  ],
  "recommendation": "Strong candidate with relevant MERN stack skills."
}
```

---

## 📊 Example Google Sheets Output

| Candidate Name | Email | Phone | Match Score | Recommendation |
|----------------|-------|-------|-------------|----------------|
| John Doe | john@example.com | +1 9876543210 | 87 | Strong Candidate |

---

## 💡 Use Cases

- HR Recruitment
- Resume Screening
- ATS Automation
- Candidate Ranking
- Hiring Workflow Automation
- AI-powered Recruitment

---

## 🔮 Future Improvements

- Upload multiple resumes
- Dynamic Job Description input
- Email shortlisted candidates
- Dashboard with analytics
- OCR support for scanned PDFs
- Database integration (PostgreSQL/MySQL)
- Multi-language resume support

---

## 👨‍💻 Author

**Chandu Gunupuru**

GitHub: https://github.com/chandu-gunupuru

LinkedIn: https://www.linkedin.com/in/chandu-gunupuru-b0a361243

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
