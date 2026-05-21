# MASTER SOFTWARE SPECIFICATION PROMPT

You are a senior full-stack AI engineer, enterprise solution architect, UI/UX designer, and GenAI platform developer.

Your task is to build a production-quality GenAI application called:

# VividPM AI

The application must be Python-based and optimized for rapid local deployment on a laptop while maintaining professional enterprise-grade UI/UX, modular architecture, AI safety guardrails, and scalable workflow design.

The application must use:

* Python backend
* Pure HTML + CSS + JavaScript frontend
* GPT/OpenAI as backend LLM
* Chart.js for dashboards
* Local filesystem storage only
* No database
* Environment variable based API key configuration using `.env`

The application must support dynamically solving multiple problems where:

* each problem may have different input types
* each problem may require different output formats
* the number of problems/questions is configurable
* Each problem is a unique module in Project management aspect.


The application should prioritize:

* UI/UX
* AI capability
* innovation
* business value
* presentation quality
* operational safety

# HIGH LEVEL APPLICATION REQUIREMENTS

The application must support:

1. Dynamic question management
2. Synthetic data generation using GPT
3. AI-powered response generation
4. Multiple output generation formats
5. Analytical dashboard generation from CSV/Excel
6. File uploads
7. Reusable MD framework support
8. Download generated outputs
9. Local storage of generated artifacts
10. Professional responsive UI

# APPLICATION NAME

The application name:

VividPM AI

must appear prominently:

* on home page
* header section
* browser title
* README
* loading screen if applicable
* Use the term “Modules” instead of problems / challenges in the UI

# FRONTEND REQUIREMENTS

Use:

* Pure HTML
* CSS
* Vanilla JavaScript

The UI theme must:

* use light pleasant colors
* appear professional
* look modern and enterprise-grade
* use responsive layouts
* support laptop screens cleanly
* avoid dark or cluttered themes

Recommended colors:

* white
* light blue
* light gray
* subtle gradients
* professional card layouts

Use:

* modern tiles/cards
* smooth transitions
* hover effects
* dashboard-style layouts
* visually appealing spacing

# APPLICATION PAGES

The application must contain:

## 1. Home Page

The homepage must:

* display application title
* display configurable question tiles/cards
* dynamically render N number of questions / module
* each tile should show:

  * question / module number
  * question / module title
  * status indicator

Clicking a tile must open the corresponding workspace page.

## 2. Configuration Page

The configuration page must allow:

* defining number of questions / modules
* defining title for each question / module
* saving configuration locally
* editing existing configuration

Store configuration in local JSON file.

## 3. Workspace Page per Question

Each question workspace must support:

### Upload Inputs

Allow upload of:

* TXT
* MD
* CSV
* XLSX
* PDF
* DOCX
* Images

### Input Description

Allow users to:

* describe scenario
* describe expected output
* describe transformation requirements

### MD Framework Upload

Allow upload of reusable `.md` instruction files.

### Synthetic Data Generation

Provide:

* button to generate synthetic input data only if required. 
* Give an option to skip synthetic data generation if not required.
* The option can be mentioned when the problem / module is configured.
* GPT-powered generation workflow

### AI Output Generation

Provide:

* Generate Output button
* progress indicator
* loading spinner

# OUTPUT TYPES SUPPORTED

The application must support generating:

* Email responses
* Knowledge documents
* HTML dashboards
* Infographics
* PPT content
* PDF-ready content
* Markdown outputs
* Analytical dashboards
* Executive summaries
* Governance documents
* Meeting transcripts
* Financial reports
* HR responses

# DASHBOARD REQUIREMENTS

When uploaded input is CSV/XLSX:

Generate interactive analytical dashboards using:

* HTML
* CSS
* JavaScript
* Chart.js

Dashboard features:

* KPI cards
* slicers
* timeline filters
* charts
* executive summaries
* risk analysis
* drill-down insights
* downloadable HTML output

# AI WORKFLOW REQUIREMENTS

The workflow should be:

User Input
↓
Scenario Understanding
↓
Synthetic Data Generation
↓
Prompt Construction
↓
LLM Invocation
↓
Output Generation
↓
Preview
↓
Download Output

# GPT INTEGRATION REQUIREMENTS

Use:

* OpenAI GPT API

The API key must:

* be loaded from `.env`
* never hardcoded
* support local development

Use environment variables:
OPENAI_API_KEY=

# BACKEND REQUIREMENTS

Use Python backend.

Recommended framework:

* Flask

The backend must support:

* file upload handling
* prompt orchestration
* OpenAI API integration
* output generation
* local file storage
* static file serving

# LOCAL STORAGE REQUIREMENTS

Do NOT use a database.

Use filesystem-based storage.

Recommended folders:

/uploads
/generated
/config
/templates
/prompts
/md_frameworks
/logs

Store:

* uploaded files
* generated outputs
* synthetic datasets
* generated dashboards
* generated markdown
* generated HTML

# REUSABLE MD FRAMEWORK SUPPORT

The application must support uploading reusable `.md` files that define:

* governance rules
* formatting guidance
* business context
* tone instructions
* dashboard requirements
* AI behavior constraints

The application must inject uploaded MD files into GPT prompts dynamically.

# OUTPUT DOWNLOAD REQUIREMENTS

Users must be able to download:

* generated HTML
* generated MD
* generated TXT
* generated CSV
* generated dashboards
* generated summaries

# SAFETY & GUARDRAILS

Implement production-quality AI safety controls.

The system must:

* validate prompts
* prevent malicious prompt injection
* sanitize uploaded file names
* validate file sizes
* prevent executable uploads from execution
* avoid exposing API keys
* limit dangerous outputs

Add guardrails against:

* prompt injection
* unsafe HTML execution
* unrestricted file access
* arbitrary code execution

# PROMPT ENGINEERING REQUIREMENTS

Create modular prompt builders.

Use:

* system prompts
* instruction prompts
* scenario prompts
* MD framework injection
* output format templates

Prompt orchestration must be modular and reusable.

# USER EXPERIENCE REQUIREMENTS

The UI must include:

* upload progress
* loading indicators
* toast notifications
* success/error alerts
* preview panels
* responsive layouts

# FILE PREVIEW SUPPORT

Support preview for:

* text files
* markdown
* generated HTML
* generated summaries

# SAMPLE QUESTION WORKFLOW

Example:

Question:
Create synthetic HR payroll complaint email and generate HR response.

Workflow:

1. User uploads scenario
2. User uploads MD framework
3. If user has opted to generated synthetic data , the uer clicks Generate Synthetic Data
4. GPT generates synthetic employee email if opted.
5. User clicks Generate Response
6. GPT generates HR response
7. User downloads generated output

# APPLICATION ARCHITECTURE

Use layered architecture:

Frontend UI Layer
↓
API Layer
↓
Prompt Orchestration Layer
↓
LLM Service Layer
↓
File Storage Layer

# REQUIRED FILES TO GENERATE

Generate all production-ready code files including:

* app.py
* requirements.txt
* .env.example
* README.md
* static CSS
* static JS
* HTML templates
* Flask routes
* utility modules
* prompt orchestration modules
* upload handling modules
* dashboard generation modules

# README REQUIREMENTS

Create a detailed README.md containing:

## Overview

## Features

## Architecture

## Folder Structure

## Setup Instructions

## Environment Setup

## Running Locally

## Sample Usage

## Supported File Types

## Troubleshooting

## Security Notes

# LOCAL SETUP REQUIREMENTS

The README must include:

## Python version

## Virtual environment creation

## pip install instructions

## .env configuration

## Running Flask server

## Accessing browser URL

# REQUIREMENTS.TXT

Include all required dependencies.

# ERROR HANDLING REQUIREMENTS

Add robust error handling for:

* API failures
* upload failures
* invalid file types
* malformed CSV
* OpenAI failures
* timeout scenarios

# PERFORMANCE REQUIREMENTS

Optimize for:

* fast local execution
* lightweight deployment
* minimal dependencies
* smooth UI interaction

# CODE QUALITY REQUIREMENTS

Generate:

* modular code
* clean architecture
* reusable functions
* comments
* production-quality naming conventions

# UI/UX REQUIREMENTS

The UI should look:

* premium
* innovative
* hackathon-demo friendly
* executive-friendly

Use:

* professional cards
* clean typography
* modern spacing
* polished dashboard styling
* Do not use the word “Hackathon” anywhere in the UI

# FINAL DELIVERABLE REQUIREMENTS

Generate:

1. Full project folder structure
2. Complete source code
3. All frontend files
4. All backend files
5. README
6. Setup instructions
7. Sample prompts
8. Sample MD frameworks
9. Example generated outputs
10. Example dashboard template

Ensure the application can be:

* cloned locally
* configured quickly
* run within minutes
* demonstrated effectively during hackathon judging

The output must be complete, implementation-ready, modular, and production-quality. Verify all output file format after building the application and as part of your testing.
