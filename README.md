# CareerPrep Job-Hunting Agent

A file-driven AI agent that helps students manage their complete
job search workflow — from resume tailoring to interview preparation
and application tracking.

---

## Student Information

- **Name:** Sadaf Tahir
- **Roll Number:** 22F-3195
- **Section:** BAI-8A
- **GitHub Username:** SadfTahir
- **Repository:** 

---

## What This Agent Does

This agent reads real job posters, resumes, and interview knowledge
base files from organized folders and performs the following tasks:

- Reads and analyzes job descriptions from input_jobs/
- Reads and analyzes student resume from input_resumes/
- Reads interview preparation notes from input_kb/
- Extracts required skills from job posters
- Extracts existing skills from resume
- Generates a skill-gap report with match percentage
- Generates tailored resume improvement suggestions
- Generates interview questions based on KB and job skills
- Maintains a job application tracker in CSV format
- Generates smart reminders with urgency levels

---

## How to Run

### Step 1 — Clone the Repository
git clone https://github.com/[your-username]/job-hunting-agent
cd job-hunting-agent

### Step 2 — Add Your Input Files
- Place job descriptions in input_jobs/ as .txt files
- Place your resume in input_resumes/ as .txt file
- Place interview notes in input_kb/ as .txt file

### Step 3 — Run the Agent
python app.py

---

## Folder Structure

job-hunting-agent/
├── app.py                  # Main agent code
├── README.md               # Project documentation
├── reflection.md           # Personal reflection
├── requirements.txt        # Python libraries
│
├── input_jobs/             # Job descriptions go here
│   ├── job_poster_01.txt
│   └── job_poster_02.txt
│
├── input_resumes/          # Your resume goes here
│   └── my_resume.txt
│
├── input_kb/               # Interview prep notes go here
│   └── interview_notes.txt
│
├── outputs/                # All generated reports saved here
│   ├── job_analysis_report.txt
│   ├── skill_gap_report.txt
│   ├── tailored_resume_suggestions.txt
│   ├── interview_questions.txt
│   └── final_agent_report.txt
│
├── tracker/                # Application tracker files
│   ├── applications.csv
│   └── reminders.txt
│
└── samples/                # Sample input files for testing
    └── sample_job_poster.txt

---

## Output Files Generated

| File | Description |
|------|-------------|
| job_analysis_report.txt | Skills and keywords found in job posters |
| skill_gap_report.txt | Match score and missing skills |
| tailored_resume_suggestions.txt | Resume improvement suggestions |
| interview_questions.txt | Technical, HR, and KB-based questions |
| final_agent_report.txt | Complete combined agent report |
| tracker/applications.csv | Application status tracker |
| tracker/reminders.txt | Interview and follow-up reminders |

---

## Application Tracker Fields

The tracker maintains the following fields for each application:

- application_id
- company
- role
- source (LinkedIn, Rozee, WhatsApp etc.)
- status (Not Applied, Applied, Shortlisted, Interview Scheduled, Rejected, Offered)
- applied_date
- interview_date
- follow_up_date
- next_action
- notes

---

## Reminder Urgency System

The agent generates smart reminders based on dates:

- OVERDUE — interview or follow-up date has p
