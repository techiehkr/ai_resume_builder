
### 📄 AI Resume Generator
Automatically generate an optimized, modern resume from raw resume text and a job description. This app extracts relevant content, enhances it based on job context, and outputs a beautiful .docx resume – optionally with a circular profile image.

## 🚀 Features
## ✅ Extracts:

Name, Role, Email, Phone, GitHub

Skills from Job Description using spaCy NLP

Experience and Education from resume text

## ✅ Builds:

A modern .docx resume (Microsoft Word)

Circular profile image if uploaded

ATS-optimized Professional Summary and Skills Section

## ✅ Streamlit Web App:

Simple UI to paste resume text and job description

File uploader for optional profile photo

## "📥 Download Resume" button to export result

## 🛠️ How it Works
Input Resume Text
Paste your resume content as plain text.

Input Job Description
Paste the job posting you're applying for.

(Optional) Upload Profile Picture
Upload a JPG/PNG image — it will be added as a circular photo on the resume.

Click Generate
A .docx file is created with:

Extracted contact info

Rewritten summary using JD keywords

Sorted bullet list of skills

Experience & education from resume

## 📦 Dependencies
Install required packages:


$ pip install -r requirements.txt
Example requirements.txt:


streamlit
python-docx
spacy
Pillow
Download spaCy English model:


''' python -m spacy download en_core_web_sm '''
💡 Example
Input:

Resume Text:


John Doe
Software Developer
johndoe@gmail.com | +91-1234567890 | github.com/johndoe

Skills:
Python, Django, SQL

Experience:
Backend Developer
ABC Corp, 2020–2023

Education:
B.Tech, Computer Science
XYZ University, 2020
Job Description: "Looking for a Python Developer with Django, REST API, PostgreSQL experience."

Output:

New resume .docx with:

Circular photo (if uploaded)

Enhanced Summary and Skills

Experience and Education auto-parsed

🖥️ Run the App

''' streamlit run .\resume_builder.py '''
📁 Output Sample
Section	Description
Summary	Uses keywords from JD in a strong summary paragraph
Skills	Auto-extracted & sorted bullet points
Experience	Preserved from input text
Education	Preserved from input text
