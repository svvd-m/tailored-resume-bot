# Tailored Resume and Cover Letter Generator

This project is a simple tool that helps job seekers create a **tailored resume** and a **cover letter**.  
It takes your original PDF resume and a job description, and then produces a clean, ATS-friendly version in a natural and human style.

The tool runs through a small Gradio web app and works with an OpenAI API key.

---

## Features

### **ATS-Friendly Output**
- Produces plain-text resumes
- Clean section headings (capital letters)
- Simple bullet points
- No special formatting that breaks ATS systems

### **Detail Preservation**
- Reads your full resume from PDF using PyPDF2  
- Keeps all information  
- Reorganises the content into a clean, simple layout

### **Custom Tailoring**
- Adds keywords from the job description  
- Highlights matching skills  
- Focuses on the role and industry requirements  

### **Natural Human Tone**
- Avoids robotic or overly formal tone  
- Makes the resume easy to read  
- Keeps a simple and confident writing style  

### **Interactive Web Interface (Gradio)**
- Works in any modern browser  
- Easy upload of:
  - resume PDF  
  - job description  
  - company info  

---

## Requirements

- **Python 3.x**
- **OpenAI API Key**  
  Store it in Colab under the secret name:  
  `openai`
- **Python Libraries**
  - `gradio`
  - `openai==0.28`
  - `PyPDF2`

---

## Installation

### **1. Clone the repository**

```bash
git clone https://github.com/your-username/tailored-resume-bot.git
cd tailored-resume-bot
```

### **2. API Key Setup**

In Google Colab, go to
Runtime → Manage Secrets → Add secret
Add your OpenAI key under the name:
```bash
openai
```
The script loads it automatically.

## Usage
Run the application
```bash
python tailored_resume_bot.py
```
After it starts, you will get a shareable Gradio link.
Open it in your browser.

Inside the Gradio interface:
- Job Description: paste the JD text
- Company Details: write company information
- Resume PDF: upload your original resume

Click submit and the tool will generate:
- a tailored resume
- a cover letter written in simple human English
Both are optimized for ATS scanning.

## Skills Demonstrated
- PDF text extraction
- Prompt engineering
- Resume tailoring logic
- ATS-friendly formatting
- Gradio interface building
- Working with OpenAI API
- Simple Python scripting
