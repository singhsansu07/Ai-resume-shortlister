# Ai-resume-shortlister
AI Resume Shortlister is an NLP-based recruitment assistance system that automatically analyzes and ranks multiple resumes according to a given job description. It helps identify relevant candidates by combining semantic similarity and skill matching instead of relying only on basic keyword searches.

Instead of relying only on exact keyword matching, the system compares the overall meaning of a candidate's resume with the job requirements. It also identifies relevant skills, missing skills, calculates an explainable match score, and generates a ranked list of candidates.

## Key Features

* Upload multiple resumes simultaneously.
* Supports **PDF, DOCX, and TXT** formats.
* Extracts text automatically from resumes.
* Detects technical and professional skills.
* Uses **Sentence Transformers** for semantic similarity.
* Compares resume content with the job description.
* Calculates a combined candidate score.
* Identifies matched and missing skills.
* Automatically ranks candidates.
* Marks candidates as **Shortlisted** or **Review**.
* Exports the final ranking to CSV.
* Provides an interactive **Gradio web interface**.
* Fully compatible with **Google Colab**.

## Scoring Method

The candidate score is calculated using:

**Final Score = 70% Semantic Match + 30% Skill Match**

### Semantic Match — 70%

A Sentence Transformer model converts the resume and job description into embeddings and measures their semantic similarity.

### Skill Match — 30%

The system detects required skills from the job description and checks which of those skills are present in each resume.

The system also displays the skills that are missing from each candidate's resume.

## Technologies Used

* **Python**
* **Natural Language Processing (NLP)**
* **Sentence Transformers**
* **Machine Learning**
* **PyMuPDF**
* **python-docx**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Gradio**
* **Google Colab**

## System Workflow

```text
Job Description
       ↓
Resume Upload
       ↓
PDF/DOCX Text Extraction
       ↓
Text Preprocessing
       ↓
Skill Extraction
       ↓
Sentence Transformer Embeddings
       ↓
Semantic Similarity
       ↓
Skill Matching
       ↓
Final Score Calculation
       ↓
Candidate Ranking
       ↓
Shortlist / Review
       ↓
CSV Report
```

## Example Output

The system produces a ranked table containing:

* Candidate Name
* Resume File
* Email
* Phone
* Final Score
* Semantic Match
* Skill Match
* Matched Skills
* Missing Skills
* Resume Skills
* Shortlist Status

## Future Improvements

Future versions can include:

* OCR support for scanned resumes
* Experience and education extraction
* Named Entity Recognition
* LLM-based resume analysis
* Candidate database
* Recruiter login and dashboard
* REST API
* Docker deployment
* Cloud deployment
* Advanced job-role-specific skill databases

## Project Objective

The main objective of this project is to demonstrate how **AI and NLP can be applied to automate resume analysis and candidate-job matching**, while providing recruiters with an explainable ranking system that can assist human review.

> This project is intended as a technical portfolio and decision-support prototype. Automated screening should not replace human judgment, and real candidate resumes containing personal information should not be uploaded to a public repository.
