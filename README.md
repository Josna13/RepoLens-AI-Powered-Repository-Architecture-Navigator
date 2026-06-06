# RepoLens AI – AI-Powered Repository Architecture Navigator

## Overview

RepoLens AI is an intelligent repository analysis platform that helps developers understand large and unfamiliar codebases in seconds instead of days.

By simply providing a public GitHub repository URL, RepoLens automatically clones the repository, performs static analysis, extracts dependency relationships, and generates an interactive architecture visualization. The platform also integrates AI-powered assistance to explain project structure, answer questions, and generate onboarding guides for new contributors.

---

## Problem Statement

Modern software projects often contain hundreds or thousands of files, making onboarding and code exploration difficult.

Developers frequently struggle with:

* Understanding project architecture
* Finding important entry points
* Tracing dependencies between modules
* Reviewing large codebases efficiently
* Estimating the impact of code changes

Traditional tools provide file navigation but fail to deliver a complete architectural understanding of the system.

---

## Solution

RepoLens AI transforms any GitHub repository into an interactive architecture map enriched with AI-powered insights.

The platform enables developers to:

* Visualize repository structure
* Understand dependencies between files
* Explore architecture interactively
* Generate onboarding guides
* Chat with the codebase using natural language
* Analyze potential change impact before modifications

---

## Key Features

### Interactive Architecture Visualization

* 2D and 3D dependency graph views
* Zoomable and interactive node exploration
* Repository-wide structural overview

### AI-Powered Code Understanding

* Repository summaries
* Module explanations
* Natural language question answering
* Context-aware codebase chat

### Dependency Analysis

* Import/export relationship mapping
* Dependency tracing
* Configuration file integration

### Developer Onboarding Assistant

* AI-generated learning paths
* Recommended file exploration order
* Faster project onboarding

### Blast Radius Analysis

* Identify files affected by modifications
* Understand downstream dependencies

### Repository Search

* Search files and code content
* Semantic repository exploration

---

## Technology Stack

### Frontend

* React
* Vite
* Tailwind CSS
* React Router DOM
* Framer Motion
* react-force-graph-3d
* react-cytoscapejs
* three-spritetext
* Lucide React

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* Madge
* simple-git
* glob

### AI Integration

* Google Gemini API
* OpenAI API
* Groq API

---

## System Architecture

User Input GitHub Repository URL

↓

Repository Cloning

(simple-git)

↓

Static Analysis

(Madge + Config Scanner)

↓

Dependency Graph Generation

↓

MongoDB Cache Storage

↓

AI Analysis Engine

↓

Interactive Dashboard

↓

Chat, Search & Onboarding Features

---

## Project Workflow

### Step 1 – Repository Submission

The user submits a public GitHub repository URL.

### Step 2 – Repository Cloning

The backend performs a shallow clone of the repository using simple-git.

### Step 3 – Static Analysis

Madge analyzes the source code and extracts dependency relationships.

### Step 4 – Graph Construction

Nodes and edges are generated to represent the repository architecture.

### Step 5 – AI Processing

The AI engine generates:

* Repository summary
* Onboarding guide
* Architecture explanations

### Step 6 – Dashboard Visualization

The frontend renders:

* Dependency graph
* File explorer
* AI assistant
* Analysis panels

---

## Project Structure

RepoLens-AI/

├── backend/

│ ├── controllers/

│ ├── routes/

│ ├── services/

│ ├── models/

│ ├── utils/

│ └── server.js

│

├── frontend/

│ ├── components/

│ ├── services/

│ ├── assets/

│ └── App.jsx

│

└── README.md

---

## Installation

### Clone Repository

```bash
git clone https://github.com/Josna13/repolens-ai.git
cd repolens-ai
```

### Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file:

```env
PORT=5000

MONGODB_URI=your_mongodb_connection_string

GEMINI_API_KEY=your_gemini_api_key

OPENAI_API_KEY=your_openai_api_key

GROQ_API_KEY=your_groq_api_key
```

Start backend:

```bash
npm run dev
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## Usage

1. Open the application.
2. Paste a public GitHub repository URL.
3. Click Analyze.
4. Explore the dependency graph.
5. Chat with the repository using AI.
6. Generate onboarding guides.
7. Analyze change impact.

---

## Future Enhancements

* Multi-language repository support
* Pull Request impact analysis
* Security vulnerability scanning
* Team collaboration features
* Repository comparison engine
* Architecture export reports

---

## Benefits

* Faster developer onboarding
* Improved architecture understanding
* Reduced code exploration time
* Better dependency visibility
* AI-assisted learning experience

---


This project is licensed under the MIT License.
