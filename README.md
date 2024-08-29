# CrewAI Agent - Tech job tailored-CV creator

This repository contains code for a Job Application Assistant that uses AI agents to streamline and enhance the job application process. The assistant is built using the crew.ai library, which allows for the creation of specialized agents tasked with specific parts of the job application journey. The agents work together as a crew to produce tailored resumes, comprehensive profiles, and interview preparation materials.

##Overview
This assistant is designed to help job applicants by automating several critical steps in the application process:

1. Researching Job Requirements: Extracting key skills, experiences, and qualifications from job postings.
2. Profiling Candidates: Compiling detailed personal and professional profiles based on provided data.
3. Tailoring Resumes: Aligning resumes with job requirements to make the application stand out.
4. Preparing for Interviews: Developing interview questions and talking points based on the resume and job requirements.

##How It Works
The assistant operates through a set of AI agents, each with a specific role:

- Tech Job Researcher: Analyzes job postings to extract relevant information.
- Personal Profiler: Compiles comprehensive profiles from various data sources.
- Resume Strategist: Tailors the resume to highlight the most relevant skills and experiences.
- Interview Preparer: Creates interview questions and talking points based on the tailored resume.

##Setting up the API Keys
To use this assistant, you'll need to provide your OpenAI API key and Serper API key. These can be set up as follows:

python
Copy code
import os
from google.colab import userdata

os.environ["OPENAI_API_KEY"] = userdata.get('OPENAI_API_KEY')
os.environ["OPENAI_MODEL_NAME"] = 'gpt-4o-mini'
os.environ["SERPER_API_KEY"] = userdata.get('OPENAI_API_KEY')

##Notes
- The agents are equipped with a set of tools, including web scraping, file reading, and semantic search, to effectively perform their tasks.

##Output Files
- **tailored_resume.md**: A resume tailored to the job requirements.
- **interview_materials.md**: A document containing potential interview questions and talking points.
