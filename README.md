# 🤖 AI ATS Resume Analyzer

## 📌 Project Overview

AI ATS Resume Analyzer is an automated recruitment workflow built with n8n, Google Gemini AI, Google Drive, Google Sheets, and Gmail.

The system automatically processes submitted resumes, extracts candidate information, evaluates qualifications using AI, categorizes applicants based on predefined criteria, generates assessment reports, and sends hiring decisions via email.

This automation significantly reduces manual resume screening time while maintaining consistent candidate evaluation.

---

## 🎯 Objectives

- Automate resume screening
- Reduce recruiter workload
- Standardize candidate evaluation
- Improve hiring efficiency
- Generate AI-powered candidate assessments

---

## 🏗️ System Architecture

```text
Google Sheets Trigger
          │
          ▼
     Download Resume
          │
          ▼
     Extract PDF Text
          │
          ▼
      Gemini AI
      Analysis
          │
          ▼
  Candidate Scoring
          │
          ▼
     Decision Logic
      /     |     \
     /      |      \
Shortlist Review Reject
    │        │      │
    ▼        ▼      ▼
Generate Generate Generate
 Report    Report   Report
    │        │      │
    ▼        ▼      ▼
 Gmail    Gmail   Gmail
````

---

## ⚙️ Workflow Implementation

### 1. Google Sheets Trigger

Monitors incoming applicant submissions.

Captured Information:

* Applicant Name
* Email Address
* Resume File URL
* Position Applied

---

### 2. Resume Retrieval

Downloads resumes automatically from Google Drive.

Supported Format:

* PDF

---

### 3. Resume Parsing

Extracts text content from uploaded resumes.

Extracted Information:

* Education
* Skills
* Certifications
* Experience
* Projects

---

### 4. AI Candidate Analysis

Uses Google Gemini AI to evaluate candidates.

Evaluation Criteria:

* Technical Skills
* Education
* Work Experience
* Certifications
* Project Experience
* Job Relevance

---

### 5. Candidate Classification

Applicants are automatically categorized into:

| Category        | Description                        |
| --------------- | ---------------------------------- |
| ✅ Shortlisted   | Meets hiring requirements          |
| ⚠️ Under Review | Requires manual evaluation         |
| ❌ Rejected      | Does not meet minimum requirements |

---

### 6. Report Generation

Creates detailed ATS evaluation reports.

Report Contents:

* Candidate Summary
* Skill Match Analysis
* Strengths
* Weaknesses
* ATS Score
* Recommendation

---

### 7. Email Notification

Sends personalized hiring results through Gmail.

Email Types:

* Shortlisted Notification
* Under Review Notification
* Rejection Notification

---

## 🧠 AI Prompt Strategy

The AI model evaluates:

* Resume quality
* Skill alignment
* Experience relevance
* Education background
* Project portfolio

Output:

* ATS Score
* Candidate Summary
* Recommendation
* Hiring Category

---

## 🧠 Skills Demonstrated

* n8n Workflow Automation
* AI Integration (Google Gemini)
* Resume Parsing & Analysis
* Applicant Tracking Systems (ATS)
* Process Automation
* Google Sheets Automation
* Google Drive Integration
* Gmail Automation
* Decision Logic Design
* JSON Data Processing
* Prompt Engineering
* Workflow Debugging

---

## 🔧 Tech Stack

### Automation

* n8n

### AI

* Google Gemini

### Storage

* Google Sheets
* Google Drive

### Communication

* Gmail

### Data Processing

* PDF Text Extraction
* JavaScript

---

## 📁 Project Structure

```text
ai-ats-resume-analyzer/
│
├── workflows/
│   └── ats-resume-analyzer.json
│
├── docs/
│   ├── architecture.png
│   ├── workflow-diagram.png
│   └── implementation-guide.md
│
├── assets/
│   └── screenshots/
│
├── README.md
└── .gitignore
```

---

## 🚀 Key Features

✅ Automated Resume Screening

✅ AI-Powered Candidate Evaluation

✅ ATS Scoring System

✅ Candidate Classification

✅ Automated Report Generation

✅ Email Notifications

✅ Scalable Recruitment Workflow

---

## 🎓 Lessons Learned

Through this project, I gained experience in:

* Building end-to-end recruitment automation workflows
* Integrating AI into HR processes
* Designing decision-based workflow routing
* Extracting and processing PDF data
* Creating scalable ATS solutions
* Implementing automated reporting systems
* Improving workflow reliability through testing and debugging
* Using prompt engineering to generate consistent candidate evaluations

---

## 📈 Impact

This solution automates the most time-consuming stages of recruitment, allowing hiring teams to focus on interviewing qualified candidates rather than manually reviewing every resume.

The workflow demonstrates how AI and automation can improve recruitment efficiency, consistency, and scalability.

---

## 📜 License

MIT License

---

## 👨‍💻 Author

Developed using n8n, Google Gemini AI, Google Workspace, and workflow automation best practices.

```
> Built an AI-powered ATS Resume Analyzer using n8n and Google Gemini that automatically screens resumes, scores candidates, generates evaluation reports, and sends hiring decisions through an end-to-end recruitment automation workflow.
```
