# 🚀 Career Catalyst: AI-Powered Career Assistant

![Java](https://img.shields.io/badge/Backend-Java%20Spring%20Boot-orange)
![Frontend](https://img.shields.io/badge/Frontend-React%20%7C%20TypeScript-blue)
![AI](https://img.shields.io/badge/AI-Google%20Gemini%20Pro-green)
![Build](https://img.shields.io/badge/Build-Maven-red)

**Career Catalyst** is an enterprise-grade, full-stack application designed to bridge the gap between job seekers and their dream roles using Generative AI. 

It solves the "Black Hole" problem of Applicant Tracking Systems (ATS) by providing real-time resume optimization, keyword gap analysis, and automated document generation using **Java Spring Boot**, **Python**, and **LaTeX**.

---

## ✨ Key Features

### 1. 📄 Intelligent Resume Builder (LaTeX Engine)
- Creates professional, ATS-friendly PDF resumes using server-side **LaTeX compilation**.
- Ensures perfect formatting and structure that standard Word parsers cannot break.
- Offers multiple industry-standard templates (Elegant, Modern, Professional).

### 2. 🤖 AI Resume Tailor (The "ATS Hacker")
- **Input:** Your Current Resume + Target Job Description (JD).
- **Process:** Analyzing the semantic gap between your skills and the JD.
- **Output:** A rewritten, keyword-optimized resume json/pdf that aligns perfectly with the role.

### 3. 🔍 Deep ATS Evaluation
- Provides a **Match Score (0-100%)** indicating your probability of getting shortlisted.
- Lists **Missing Keywords** and critical hard/soft skills.
- Offers actionable feedback to improve content quality.

### 4. ✍️ Contextual Cover Letter Generator
- Generates personalized cover letters by analyzing the tone of the company's JD and your specific achievements.
- Eliminates generic "To Whom It May Concern" templates.

### 5. 🎤 AI Mock Interviewer
- Generates role-specific interview questions based on the JD.
- Helps candidates prepare for technical and behavioral rounds.

---

## 🏗️ System Architecture

The application follows a **Hybrid Microservices-inspired Architecture**:

1.  **Frontend (Client):** React.js with TypeScript handles user interaction and state management.
2.  **API Layer (Gateway):** **Spring Boot** (Java) serves as the robust backend, handling REST API requests, file storage, and business logic.
3.  **Intelligence Layer:** Java triggers specialized **Python Scripts** via `ProcessBuilder`.
4.  **GenAI Integration:** Python scripts communicate with **Google Gemini API** for reasoning and content generation.
5.  **Document Engine:** The backend compiles `.tex` files into PDFs using a local LaTeX distribution.

---

## 🛠️ Tech Stack

### Backend
* **Language:** Java 17+
* **Framework:** Spring Boot 3.x (Web, REST)
* **Build Tool:** Maven
* **PDF Engine:** LaTeX (TeX Live / MiKTeX)

### Frontend
* **Library:** React.js (v18)
* **Language:** TypeScript
* **Styling:** CSS Modules / Custom CSS
* **HTTP Client:** Axios

### AI & Scripting
* **Language:** Python 3.x
* **LLM:** Google Gemini Pro
* **Libraries:** `google-generativeai`, `requests`

---

## 🚀 Getting Started

Follow these instructions to set up the project locally.

### Prerequisites
Ensure you have the following installed:
* **Java JDK 17+**
* **Node.js & npm**
* **Python 3.8+**
* **Maven**
* **LaTeX Distribution:**
    * *Windows:* Install [MiKTeX](https://miktex.org/download) (Required for PDF generation).
    * *Linux:* `sudo apt-get install texlive-full`

### Installation Guide

#### 1. Clone the Repository
```bash
git clone [https://github.com/MohdArshad-cell/ai-powered-career-catalyst.git](https://github.com/MohdArshad-cell/ai-powered-career-catalyst.git)
cd ai-powered-career-catalyst

```

#### 2. Backend Setup

Navigate to the backend directory and configure the environment:

```bash
cd backend
# Install Python dependencies for the AI engine
pip install -r src/main/resources/scripts/requirements.txt

```

**Configure API Key:**
Open `src/main/resources/application.properties` (or set as Environment Variable) and add your Gemini API Key:

```properties
gemini.api.key=YOUR_GOOGLE_GEMINI_API_KEY
file.upload-dir=./uploads

```

Run the Spring Boot Server:

```bash
mvn spring-boot:run

```

*Server will start at `http://localhost:8080*`

#### 3. Frontend Setup

Open a new terminal and navigate to the frontend directory:

```bash
cd frontend
npm install
npm start

```

*Client will open at `http://localhost:3000*`

---

## 📸 Usage Workflow

1. **Select a Template:** Choose a resume design.
2. **Input Data:** Fill in profile, education, and projects (or upload existing JSON).
3. **Tailor:** Paste the Job Description of the role you want.
4. **Generate:** Click "Download PDF". The backend orchestrates Java, Python, and LaTeX to deliver the file.

---

## 📬 Contact & Support

Developed by **Mohd Arshad**.

* **Email:** [arshadmohd8574@gmail.com](mailto:arshadmohd8574@gmail.com)
* **LinkedIn:** [Mohd Arshad](https://www.linkedin.com/in/mohd-arshad-156227314/)
* **GitHub:** [MohdArshad-cell](https://github.com/MohdArshad-cell)

---

*Note: This project is a demonstration of Polyglot Programming (Java + Python) and System Design capabilities for educational purposes.*
Bas isko paste kar aur commit kar de! GitHub profile chamak jayegi.
