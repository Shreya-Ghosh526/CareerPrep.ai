# CareerPrep.AI – Personalized Mock Interview System

CareerPrep.AI is a cloud-native AI-powered platform that delivers hyper-personalized technical mock interviews by analyzing a user’s GitHub repositories and resume.

Unlike generic interview platforms, CareerPrep.AI generates interview questions based on the candidate’s actual code, architecture decisions, and project implementations.

---

## 🚀 Problem Statement

Students often prepare for interviews using generic coding platforms, but real interviewers ask deep questions about:

- Their own projects
- Architectural decisions
- Technology choices
- Trade-offs and design reasoning

This gap leads to lack of confidence and poor performance in real interviews.

CareerPrep.AI solves this by simulating realistic, project-specific mock interviews.

---

## 🎯 Key Features

### 1️⃣ Resume & GitHub Integration
- Upload Resume (PDF/DOC/DOCX supported)
- Extract structured data (education, skills, projects)
- Connect GitHub account via GitHub API
- Analyze repositories and project metadata

### 2️⃣ Intelligent Code Analysis
- Detect technology stack
- Identify architectural patterns
- Extract technical decisions (database, frameworks, APIs)
- Measure project complexity
- Categorize project types

### 3️⃣ Personalized Question Generation
- Generate project-specific technical questions
- Ask about implementation decisions
- Create adaptive follow-up questions
- Avoid irrelevant or generic questions

### 4️⃣ Voice-Based Interview Simulation
- Text-to-Speech using Amazon Polly
- Speech-to-Text using Amazon Transcribe
- AI-driven conversation using Amazon Bedrock
- Real-time interaction and response evaluation

### 5️⃣ Interview Session Management
- Start / Pause / Resume / End interview
- Track question progression
- Store transcripts
- Generate performance summaries
- Provide constructive feedback

---

## 🏗️ System Architecture

CareerPrep.AI follows a microservices architecture with clear separation of concerns.

### Architecture Layers

### Frontend Layer
- React + TypeScript SPA
- Voice Interface component

### API Gateway Layer
- REST API routing
- Authentication handling

### Backend Services
- Authentication Service
- Profile Service
- Interview Service
- Code Analysis Service

### AWS Lambda Functions
- Resume Parser Lambda
- Code Analyzer Lambda
- Question Generator Lambda
- Interview Engine Lambda

### AWS AI Services
- Amazon Transcribe (Speech-to-Text)
- Amazon Polly (Text-to-Speech)
- Amazon Bedrock (AI Question Generation & Context Handling)

### Data Layer
- User Database
- Session Database
- Analysis Database
- S3 Storage

---

## 🔄 System Flow

1. User uploads resume
2. Resume Parser extracts structured data
3. User connects GitHub account
4. Code Analyzer scans repositories
5. Analysis results stored in database
6. Interview session begins
7. Questions generated via Bedrock
8. Polly speaks question
9. User responds via voice
10. Transcribe converts speech to text
11. Interview Engine evaluates and generates follow-up
12. Session summary stored and displayed

---

## 🧠 AI & AWS Integration

CareerPrep.AI leverages AWS managed services:

- Amazon Bedrock → Context-aware AI interviewer
- Amazon Transcribe → High-accuracy speech recognition
- Amazon Polly → Natural speech output

The system handles AWS service failures gracefully and includes fallback mechanisms.

---

## 📊 Data Models

### User & Profile
- ResumeData
- GitHub Repository Metadata
- Analysis Results
- Interview Sessions

### Interview Models
- Question
- Response
- Interview Summary
- Performance Metrics

---

## 🔐 Security & Data Handling

- Sensitive data encrypted
- Secure GitHub token handling
- Structured database storage
- Data retention policies supported
- Backup & availability strategies implemented

---

## 🛠️ Tech Stack

Frontend:
- React
- TypeScript

Backend:
- Node.js
- TypeScript

Cloud & AI:
- AWS Lambda
- Amazon Bedrock
- Amazon Transcribe
- Amazon Polly
- S3 Storage

External Integration:
- GitHub API

---

## 🎓 Target Users

- Students preparing for technical interviews
- Job seekers with GitHub projects
- Developers wanting realistic interview simulation

---

## 📈 Future Enhancements

- Multi-language support
- Premium analytics dashboard
- Company-specific interview simulation
- AI-based resume improvement suggestions

---

## 💡 Why CareerPrep.AI?

Because interviews aren’t about solving random problems —
they’re about explaining your own work with clarity and confidence.

CareerPrep.AI bridges the gap between preparation and real interviews.
