# SmartLoan AI

### AI-Powered Loan Application, PDF Intelligence, Review Workflow & Risk Prediction Platform

SmartLoan AI is a professional full-stack AI/ML portfolio project that demonstrates a complete digital loan-processing system with loan application management, PDF generation, document extraction, machine learning prediction, admin review workflow, reporting, AI document assistance, and Docker-based deployment.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green)
![React](https://img.shields.io/badge/React-Frontend-61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-Frontend-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-scikit--learn-orange)
![Docker](https://img.shields.io/badge/Docker-Ready-2496ED)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## Repository
**GitHub:** [https://github.com/tankim-prio/smartloan-ai](https://github.com/tankim-prio/smartloan-ai)

---

## Table of Contents
* [Project Overview](#project-overview)
* [Project Objective](#project-objective)
* [Why This Project Matters](#why-this-project-matters)
* [Core Features](#core-features)
* [Technology Stack](#technology-stack)
* [System Architecture](#system-architecture)
* [Main Application Workflow](#main-application-workflow)
* [Machine Learning Workflow](#machine-learning-workflow)
* [PDF Intelligence Workflow](#pdf-intelligence-workflow)
* [Important Pages](#important-pages)
* [Project Structure](#project-structure)
* [Local Development Setup](#local-development-setup)
* [Docker Setup](#docker-setup)
* [Health Check URLs](#health-check-urls)
* [API Areas](#api-areas)
* [Docker Persistence Design](#docker-persistence-design)
* [Screenshots](#screenshots)
* [Demo Video Flow](#demo-video-flow)
* [Recruiter and Professor Review Notes](#recruiter-and-professor-review-notes)
* [Future Improvements](#future-improvements)
* [Author](#author)
* [Project Status](#project-status)

---

## Project Overview
SmartLoan AI is a realistic loan application processing platform designed to demonstrate practical software engineering, applied AI/ML integration, document intelligence, and end-to-end workflow automation.

The system allows an applicant to create a loan application, generate a loan PDF, upload documents, extract information from PDFs, run machine learning based loan risk prediction, send the application for review, and allow an admin or reviewer to approve or refuse the application.

This project connects multiple real-world software components into one complete workflow:
* Frontend application
* Backend REST API
* Database-backed loan workflow
* PDF generation
* PDF text extraction
* OCR-based document processing
* Machine learning prediction
* Admin review system
* Dashboard and reports
* AI/RAG-style document assistant
* Dockerized deployment

---

## Project Objective
The main objective of SmartLoan AI is to simulate a real-world digital loan processing platform where user data, financial documents, machine learning prediction, document extraction, and human review are connected in one professional system.

This project is highly suitable for:
* International job recruiter review
* University project evaluation
* AI / Machine Learning Engineer portfolio
* Backend / Full-stack Developer portfolio
* Document intelligence project showcase
* Dockerized application demonstration

---

## Why This Project Matters
SmartLoan AI is not a simple CRUD application. It demonstrates how a modern fintech-style system can combine user inputs, asynchronous-feeling data processing, and analytical intelligence. Because of this, the project can be reviewed as an engineering piece across multiple domains: **AI Engineering, Machine Learning Engineering, Backend Engineering, and Workflow Automation.**

---

## Core Features

### 🔐 Authentication & User Workflow
* Secure login and account creation
* Personalized user profile management
* Role-based view logic separation (Applicant vs. Admin/Reviewer workflow)

### 📋 Loan Application Management
* Form workflow capturing Personal, Employment, Financial, and Loan details
* Dynamic draft state saving
* Clean inputs designed to process fresh application data seamlessly rather than relying on static mock examples

### 📄 PDF Generation
* Programmatic generation of comprehensive loan application documents
* Supports embedding applicant summaries, asset checklists, and space placeholders for official verification attachments

### 🔍 PDF Upload & Document Extraction
* Deep text extraction layer for native digital PDFs
* Built-in **OCR Fallback engine** to process scanned physical sheets or uploaded images (Salary certificates, NID cards, passports)
* Fully structured field mapping extracting metadata such as *Monthly Income, Designation, ID serial digits, and Employer credentials*

### ⚖️ Review Management System
* Interactive administrative board displaying Pending, Approved, and Refused requests
* Comprehensive inspection utility displaying parsed asset text alongside system recommendations

### 🤖 Machine Learning Risk Prediction
* On-the-fly **Approval Probability** mapping
* Numerical **Risk Scoring engine** segments requests into high/medium/low risk bands
* Human-readable prediction insight strings explaining the primary driving weights behind the model's logic

### 📊 Dashboard & Reports
* Exec-level interactive charts displaying pipeline velocity, loss metrics, and state counts
* Historical metrics parsing for performance evaluation

### ✈️ AI Pilot / RAG Assistant
* Localized semantic search context container using internal policy documentation
* Natural language prompt engine built to assist agents with loan eligibility rule auditing

### 🐳 Docker Deployment
* Modular orchestration breaking dependencies into specific frontend, backend, and reverse proxy containers
* Multi-stage build architectures pinning dependencies accurately

---

## Technology Stack

| Layer | Technologies |
| :--- | :--- |
| **Frontend** | React, Vite, TypeScript, Tailwind CSS, Shadcn UI paradigms |
| **Backend** | Python, FastAPI, Uvicorn, Pydantic, SQLAlchemy |
| **Database** | SQLite |
| **Machine Learning** | scikit-learn, pandas, NumPy, joblib |
| **PDF Processing** | PyPDF, PyMuPDF, ReportLab |
| **OCR / Image Processing** | pytesseract, Pillow |
| **AI Assistant** | RAG-style document assistant workflow |
| **DevOps** | Docker, Docker Compose, Nginx |
| **Storage** | Local structured storage directories bound to Docker Volume maps |

---

## System Architecture

```mermaid
flowchart TD
    A[Applicant / Admin User] --> B[React + Vite Frontend]
    B --> C[FastAPI Backend API]
    C --> D[SQLite Database]
    C --> E[File Storage]
    C --> F[PDF Generation Service]
    C --> G[PDF Extraction Service]
    C --> H[ML Prediction Service]
    C --> I[AI / RAG Document Assistant]
    D --> J[Applications, Users, Reviews]
    E --> K[Uploads, Generated PDFs, Documents]
    H --> L[Risk Score, Approval Probability, Risk Band]
    G --> M[Readable Text and Structured Fields]
