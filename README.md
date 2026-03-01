# 🤖 AI Resume Optimizer

Tailor your resume to any job description in seconds — powered by Google Gemini AI and built with Gradio on Google Colab.

---

## ✨ Features

- **PDF Upload** — Upload your resume as a PDF and auto-extract the text
- **JD Analysis** — Automatically analyzes the job description and extracts must-have skills, nice-to-haves, key responsibilities, and ATS keywords
- **Clarifying Questions** — AI identifies gaps between your resume and the JD, then asks targeted questions to surface hidden experience
- **Resume Optimization** — Rewrites your resume with the right keywords, framing, and action verbs to pass ATS filters and impress hiring managers
- **Save to Google Drive** — Save optimized resumes by job category directly to your Drive
- **Resume Library** — Browse all your saved resumes grouped by category
- **Optimization History** — Automatically logs every optimization session with a timestamp and preview

---

## 🚀 Getting Started

### Prerequisites

- A Google account with Google Colab access
- A [Gemini API key](https://aistudio.google.com/app/apikey) (free tier available)
- Google Drive mounted in Colab (for saving resumes and history)

### Setup

1. Open the notebook in Google Colab
2. Mount your Google Drive when prompted
3. Run the cell — it will install dependencies (`PyMuPDF`, `gradio`, `google-genai`) automatically
4. Paste your Gemini API key in the **Settings** panel and click **Set API Key**

---

## 🧭 How to Use

### Step 1 — Input your resume
Upload a PDF **or** paste your resume text directly into the text box.

### Step 2 — Paste the job description
Copy the full job description from the job posting and paste it into the JD field.

### Step 3 — Analyze
Click **🔍 Analyze & Generate Questions**. The AI will:
- Break down the JD into a structured summary
- Generate 2–3 targeted clarifying questions about potential gaps

### Step 4 — Answer the questions
Provide short answers to the clarifying questions. These are woven into your optimized resume — the more detail you give, the better the output.

### Step 5 — Optimize
Click **⚡ Optimize My Resume** to generate the tailored resume.

### Step 6 — Save
Use **📋 Copy to Clipboard** to grab the output, or select a job category and click **💾 Save Resume** to store it to Google Drive.

---

## 📁 File Structure (Google Drive)

```
MyDrive/
└── AI_Resume_Optimizer/
    ├── history.json               # Optimization history log
    └── resumes/
        ├── ML_Engineer/
        ├── Data_Scientist/
        ├── AI_Engineer/
        ├── Computer_Vision/
        └── Software_Engineer/
```

---

## 🗂️ Tabs

| Tab | Description |
|-----|-------------|
| ✏️ Optimizer | Main resume optimization workflow |
| 📚 Resume Library | Browse all saved resumes by category |
| 🕐 History | View a log of all past optimization sessions |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| [Google Gemini 2.5 Flash](https://deepmind.google/technologies/gemini/) | LLM for JD analysis and resume rewriting |
| [Gradio](https://gradio.app/) | Web UI framework |
| [PyMuPDF (fitz)](https://pymupdf.readthedocs.io/) | PDF text extraction |
| [Google Colab](https://colab.research.google.com/) | Cloud notebook environment |
| Google Drive | Persistent storage for resumes and history |

---

## ⚠️ Notes

- The AI will **never fabricate experience** — it only uses information from your original resume and your answers to the clarifying questions
- Image-based PDFs (scanned documents) cannot be parsed automatically — paste your resume text manually in that case
- Your Gemini API key is stored in memory only for the duration of the session

---

## 📄 License

This project is for personal use. Please review [Google Gemini's usage policies](https://ai.google.dev/gemini-api/terms) before deploying publicly.
