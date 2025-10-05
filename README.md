# ats-resume-generator
python code to generate resume
🔹 Overview

This Python project automatically generates ATS-friendly resumes tailored to real job postings. It:

Scrapes job listings from websites like Indeed or LinkedIn.

Extracts keywords and requirements from job descriptions.

Generates Word (.docx) and PDF resumes for each job.

Optimizes resumes for Applicant Tracking Systems (ATS) with proper formatting, keywords, and sections.

🔹 Features

Generates 100+ resumes automatically.

Creates role-specific resumes based on scraped job postings.

Includes key ATS-friendly sections:

Contact Information

Professional Summary

Skills

Experience

Education

Converts Word resumes to PDF format.

Randomized but realistic data using Faker for names, emails, phone numbers, and education.

🔹 Prerequisites

Python 3.10+ recommended.

Required Python libraries:

pip install requests beautifulsoup4 python-docx fpdf pandas faker docx2pdf


requests – For HTTP requests to fetch job postings.

beautifulsoup4 – To parse HTML and extract job data.

python-docx – To create Word documents.

docx2pdf – To convert Word documents to PDF.

fpdf – Optional for PDF conversion.

pandas – For CSV data handling (job roles/keywords).

faker – To generate random realistic data.

🔹 File Structure
ATS_Resume_Generator/
│
├── job_roles_keywords.csv     # CSV with roles and ATS keywords
├── main.py                    # Python script to generate resumes
├── ATS_Resumes/               # Folder where generated resumes are saved
│    ├── Resume_1_Software_Engineer.docx
│    ├── Resume_1_Software_Engineer.pdf
│    └── ...
└── README.md

🔹 CSV File Format

job_roles_keywords.csv – defines job roles and keywords:

Role	Keyword1	Keyword2	Keyword3	Keyword4	Keyword5
Software Engineer	Python	Java	Git	Agile	REST API
Data Analyst	SQL	Excel	Tableau	Analytics	Power BI
Project Manager	Project Mgmt	Scrum	Leadership	Agile	Stakeholder

Role column is mandatory.

Keywords columns are optional, but recommended for ATS optimization.

🔹 Usage

Update CSV: Add the job roles and relevant ATS keywords.

Run the script:

python main.py


Resumes Output: All resumes are saved in the ATS_Resumes/ folder in both .docx and .pdf formats.

Customization: You can adjust:

Number of resumes generated.

Skills, experience, or education templates.

Job scraping source URL.

🔹 Notes

Scraping job portals may require handling dynamic content (JavaScript). For LinkedIn or advanced websites, consider Selenium or official APIs.

Ensure legal compliance while scraping and using job postings.

The generated resumes are template-based, but realistic enough for ATS testing and demonstrations.

🔹 Future Enhancements

Automatically extract keywords from live job postings for more accurate resume tailoring.

Include cover letter generation.

Integrate with a web interface for one-click resume creation.

Add multi-language support (English + Hindi + Local Languages).
