📝 ATS Resume Generator (Python)

A Python project that automatically generates ATS-friendly resumes tailored to real job postings.
It extracts job-specific keywords and formats resumes to optimize for Applicant Tracking Systems (ATS).

🔹 Overview

Scrapes job listings from websites like Indeed or LinkedIn

Extracts keywords and requirements from job descriptions

Generates Word (.docx) and PDF resumes

Optimizes resumes with proper sections, formatting, and keywords

Randomized but realistic data using Faker

✨ Features

Generates 100+ resumes automatically

Role-specific resumes based on job postings

ATS-friendly sections included:

Contact Information
...
Professional Summary

Skills


Experience

Education

Converts Word resumes to PDF format

Randomized names, emails, phone numbers, and education using Faker

🧩 Prerequisites

Python 3.10+ recommended

Install required libraries:

pip install requests beautifulsoup4 python-docx fpdf pandas faker docx2pdf


Library Purposes:

requests – Fetch job postings

beautifulsoup4 – Parse HTML and extract job data

python-docx – Create Word documents

docx2pdf – Convert Word to PDF

fpdf – Optional PDF conversion

pandas – CSV handling (job roles/keywords)

faker – Generate realistic random data

📂 File Structure
ATS_Resume_Generator/
│
├── job_roles_keywords.csv     # CSV with roles and ATS keywords
├── main.py                    # Python script to generate resumes
├── ATS_Resumes/               # Folder for generated resumes
│    ├── Resume_1_Software_Engineer.docx
│    ├── Resume_1_Software_Engineer.pdf
│    └── ...
└── README.md

🗂️ CSV File Format

job_roles_keywords.csv defines job roles and keywords:

Role	Keyword1	Keyword2	Keyword3	Keyword4	Keyword5
Software Engineer	Python	Java	Git	Agile	REST API
Data Analyst	SQL	Excel	Tableau	Analytics	Power BI
Project Manager	Project Mgmt	Scrum	Leadership	Agile	Stakeholder

Role column is mandatory

Keyword columns are optional but recommended for ATS optimization

⚙️ Usage

Update CSV: Add job roles and relevant ATS keywords

Run the script:

python main.py


Output:
All resumes are saved in ATS_Resumes/ in both .docx and .pdf formats

Customizable Options:

Number of resumes generated

Skills, experience, or education templates

Job scraping source URL

⚠️ Notes

Scraping job portals may require handling dynamic content (JavaScript).

For LinkedIn or advanced websites, consider Selenium or official APIs.

Ensure legal compliance while scraping and using job postings.

Generated resumes are template-based but realistic enough for ATS testing.

🔮 Future Enhancements

Automatically extract keywords from live job postings for accurate tailoring

Cover letter generation

Web interface for one-click resume creation

Multi-language support (English + Hindi + Local Languages)

🏷️ Tags

#python #resume #ATS #automation #job #docx #pdf #faker #scraping #career
