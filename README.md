# FlyRank ML Internship — Starter Repo

**Applied Search Intelligence: Google Search Ranking & Discoverability**

This is the starting point for the FlyRank ML Internship. You **clone it into your own public
repo** (one click — *Use this template*), build everything there, and submit that repo URL on
each assignment in your portal — it's your workspace, your submission, and your portfolio all
at once. The rhythm is simple: do the work, commit it, submit on the card. Done.

Everything here runs on a small **anonymized** slice of real FlyRank search data. No credentials,
no private client data, no setup headaches.

> **New here?** Two reads: **[SETUP.md](SETUP.md)** (GitHub, Colab, and data access — ten
> minutes, with every silent pitfall flagged), then **[GUIDE.md](GUIDE.md)** (every file
> explained, what to edit vs. leave alone, and where your own work goes — five minutes).

---

## Quickstart — first win in 2 minutes

The fastest path is Google Colab (one click, zero install). Open Notebook 1 and run all cells:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/flyrank-bih/flyrank-ml-internship-starter/blob/main/notebooks/01_first_look_and_discovery.ipynb)
 **Week 1 — Run it, then discover a real truth yourself**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/flyrank-bih/flyrank-ml-internship-starter/blob/main/notebooks/02_your_first_readable_model.ipynb)
 **Week 2 — The model is just a rule you can read**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/flyrank-bih/flyrank-ml-internship-starter/blob/main/notebooks/03_working_with_the_full_release.ipynb)
 **Weeks 3+ — The full release (~79M rows) via DuckDB, no download needed** — hosted at
 [`FlyRank/internship-warehouse`](https://huggingface.co/datasets/FlyRank/internship-warehouse) (gated: request access + accept the data-use terms, approval is instant)

### Prefer local?

```bash
git clone <this-repo-url>
cd flyrank-ml-internship-starter
pip install -r requirements.txt          # or: uv pip install -r requirements.txt
python scripts/run_all.py
```

That runs the whole pipeline on the bundled sample and writes results to `outputs/`.

---

## What you get

| Path | What it is |
|---|---|
| `notebooks/` | Week 1–2 **first-win notebooks** (Colab-ready). Start here. |
| `scripts/01–05` + `run_all.py` | The runnable reference pipeline: prepare → baseline → train → evaluate → PDF. |
| `data/raw/content_refresh_anonymized.csv` | The anonymized starter dataset (~30k pages). |
| `outputs/` | Example outputs so you can see the **target shape** (`model_report.md`, `refresh_queue_sample.csv`, `charts/`). |
| `work/` | **Your space.** Lane experiments and your capstone live here — see `work/README.md`. |
| `docs/` | The core docs + the data dictionary (see below). |

### Read these (in `docs/`)

1. **`ml-core-foundation-framework.md`** — the first-principles map of ML as a whole system. The backbone of the live sessions.
2. **`ml-intern-dataset-and-lane-guide.md`** — how to use the data safely, the capstone workflow, and the analysis "lanes" you can pick from.
3. **`intern-free-tooling-guide.md`** — the zero-budget tool stack (Python, Colab, free AI assistants). You never need to pay for anything.
4. **`data-dictionary.md`** — all 44 columns: meaning, scale, and gotchas. Keep it open while you work.

---

## The pipeline (what `run_all.py` does)

```text
01_prepare_features.py   clean + build the feature vector, define the label
02_baseline_score.py     a transparent hand-rule "fix this first" score
03_train_model.py        logistic regression, decision tree, random forest (client-holdout split)
04_evaluate_and_export.py  ranked queue + charts + Markdown report
05_build_pdf_report.py   a shareable PDF summary
```

On the bundled sample, the learned model clearly beats the hand-written rule at picking the right
pages to review first (**Precision@50 ≈ 0.24 → 0.74**; the model number can land 0.68–0.74
depending on library versions — the ~3x lift is the point). The notebooks compute these numbers
live, so they always reflect the current data and environment.

**Teaching point:** the model is the capstone, but the *workflow* is the lesson —
`problem framing → data cleaning → baseline → first model → evaluation → explainable recommendation`.

---

## Data safety (read `DATA_USE.md`)

- Only the small **anonymized** CSV ships here — no client names, domains, URLs, titles, or keywords.
- **Never** add raw private client data to this repo or your fork. Need more data? Request an approved
  release from your mentor — never export it yourself.
- Don't paste client data into third-party AI tools.
- Frame every result as **observed / measured / directional / decision-support** — never
  "I predicted Google's algorithm."

The `.gitignore` blocks datasets by default, and CI fails any commit that includes a dataset.

---

## Assignments & schedule

Weekly assignments, live events, and the capstone live on **your portal board** (your
enrollment email has your access link). This repo is the shared technical foundation they all
build on — and the `skills/` folder here is the instruction library for your AI assistant
(start at [skills/README.md](skills/README.md)).

**First time with GitHub?** You need exactly four things (full walkthrough: [SETUP.md](SETUP.md)):
1. A free account at github.com.
2. Your own copy of this repo: **Use this template → Create a new repository** → public.
   (One click — brings the notebooks, `work/`, and the CI leak-guard with it.)
3. In Colab: *File → Save a copy in GitHub* → pick your copy, branch `main` (Colab handles auth).
4. That's your submission repo — share its **github.com/you/your-repo** URL with Assignment 1
   (never a colab.research.google.com or drive.google.com link).

---


## Week 1 Assignment Submission

### Search Question
Can we predict whether a customer will purchase a vehicle based on their profile and preferences?

### Is this an ML problem?
Yes. Customer purchasing decisions depend on many factors and patterns that cannot be captured well using simple fixed rules.

### ML Task Type
Classification

### Learning Type
Supervised Learning

### Input Features
- Age
- Income
- City
- Family Size
- Previous Purchases
- Preferred Vehicle Type

### Target Variable
Purchase Decision (Yes/No)

### Success Metrics
- Accuracy
- Precision
- Recall
- F1 Score

### Why Machine Learning?
Machine Learning can learn patterns from historical customer data and make predictions for new customers.

### Conclusion
This is a supervised machine learning classification problem.

*Track leads: Mirza Ašćerić (ML) · Hole (data engineering). Code under MIT (see `LICENSE`); data under `DATA_USE.md`.*
# FL-09: Documentation and Demo Video

## Project Title

# MVS AI Portfolio Agent

---

## 1. Project Overview

MVS AI Portfolio Agent is an interactive AI-powered portfolio feature designed to help visitors understand my profile, education, skills, projects, technical interests, and experience.

Instead of requiring visitors to search through multiple static portfolio sections, the Agent allows visitors to ask questions directly through a conversational interface.

The project demonstrates how an AI/Agent-style feature can be integrated into a personal portfolio to make the experience more interactive and easier to explore.

---

## 2. Project Purpose

The purpose of this project is to:

- Present my technical profile through a modern portfolio.
- Demonstrate practical AI/ML skills.
- Provide an interactive Agent experience.
- Allow visitors to ask questions about my background and projects.
- Demonstrate deployment of a working web project.
- Document the project clearly enough for another person to understand the workflow.

---

## 3. Intended Users

The portfolio is designed for:

- Recruiters
- Internship reviewers
- Mentors
- Developers
- Technical reviewers
- Visitors interested in AI/ML projects
- Visitors interested in my technical skills

---

## 4. Live Portfolio

The deployed portfolio is available at:

https://vasi-portfolio1.netlify.app/

---

## 5. Main Dynamic Feature

## Query My Agent

The main dynamic feature of the portfolio is the **Query My Agent** conversational interface.

Visitors can interact with the Agent and ask questions about:

- My profile
- My education
- My technical skills
- My technology stack
- My projects
- My AI/ML interests
- My portfolio work

The Agent makes the portfolio interactive rather than being only a collection of static web pages.

---

## 6. Example Questions

Example questions that can be asked to the Agent include:

- Tell me about yourself.
- What is your tech stack?
- What are your AI/ML skills?
- Tell me about your projects.
- Tell me about FinnSays.
- What technologies do you work with?
- What are your technical interests?

---

## 7. How to Use the Agent

1. Open the live portfolio.

   https://vasi-portfolio1.netlify.app/

2. Navigate to the **Agent** section.

3. Open **Query My Agent**.

4. Enter a question into the Agent interface.

5. Submit the question.

6. Read the generated response.

7. Try another question to explore additional portfolio information.

---

## 8. Data Flow

The basic data flow of the Agent is:

```text
User Question
      ↓
Portfolio Frontend
      ↓
Agent Interface / Logic
      ↓
Portfolio Information
      ↓
Response Generation
      ↓
Response Displayed to User
# Final Statement

The project demonstrates a practical AI-powered portfolio experience with a working interactive Agent.

The documentation explains the purpose, users, setup, usage, data flow, evaluation, design decision, limitations, deployment, and demonstration.

All evaluation claims are based on observed manual testing, and the Agent is presented as a portfolio assistant rather than a general-purpose AI system.
# Mohd Vasi Saifi — AI & Software Engineering Portfolio

## 🚀 Project Overview

This repository contains my personal **AI & Software Engineering Portfolio**, developed as part of my **General AI Fluency Capstone Project**.

The portfolio demonstrates my skills in:

* Artificial Intelligence & Machine Learning
* Full-Stack Web Development
* Front-End Development
* NLP and conversational agents
* Real-time data handling
* Modern web technologies
* GitHub-based development and deployment

### 🌐 Live Portfolio

**Live Website:**
https://vasi-portfolio2.netlify.app/

### 💻 GitHub Repository

**Repository:**
https://github.com/vasisaifi1-creator/project1

---

# 👨‍💻 About Me

**Name:** Mohd Vasi Saifi

**Program:** B.Tech (Hons.) in Artificial Intelligence & Machine Learning

**University:** SDGI Global University, Ghaziabad

**Expected Graduation:** 2028

I am a B.Tech AI & ML student interested in software engineering, artificial intelligence, full-stack development, intelligent agents, and practical AI applications.

My portfolio showcases my technical skills, projects, and an interactive NLP-lite conversational agent.

---

# 🎯 Capstone Project

## Building Fintech Intelligence & Intelligent Agents

The main objective of this portfolio is to demonstrate how modern web development and artificial intelligence concepts can be combined into an interactive personal engineering portfolio.

The project includes an interactive conversational agent that can answer questions about my portfolio, skills, projects, and technical background.

---

# ✨ Main Features

## 1. Responsive Portfolio Website

The website provides a clean and responsive interface containing:

* About Me
* Technical Skills
* Featured Projects
* AI Agent
* Resume Download
* Navigation Menu
* Theme Support

---

## 2. Interactive AI Agent

The portfolio contains an NLP-lite conversational agent trained using portfolio information.

Users can ask questions such as:

* What tech stack do you use?
* What projects have you built?
* What are your AI skills?
* What programming languages do you know?
* Tell me about your portfolio.
* What is your education?

The agent provides responses based on the portfolio's structured information.

### System Command

The agent also supports:

```text
/system
```

This command provides system/telemetry information.

---

# 🛠️ Technology Stack

## Frontend

* HTML5
* CSS3
* JavaScript
* Responsive Web Design

## AI / ML

* Artificial Intelligence
* Machine Learning
* Natural Language Processing
* NLP-based conversational logic

## Development Tools

* Git
* GitHub
* VS Code
* Netlify
* Google Lighthouse
* PageSpeed Insights

---

# 📁 Project Structure

```text
AI-Portfolio/
│
├── index.html
├── style.css
├── script.js
├── chatbot.js
├── README.md
│
└── assets/
    ├── profile.jpg
    └── resume.pdf
```

---

# ⚡ Performance Testing

The portfolio was tested using **Google PageSpeed Insights / Lighthouse**.

## Latest Test

**Date:** September 5, 2026

**Environment:** Desktop

**Lighthouse Version:** 13.4.1

### Results

| Category         |       Score |
| ---------------- | ----------: |
| Performance      |  **99/100** |
| Accessibility    |  **95/100** |
| Best Practices   | **100/100** |
| SEO              | **100/100** |
| Agentic Browsing |     **2/2** |

---

# 📊 Core Performance Metrics

| Metric                         |    Result |
| ------------------------------ | --------: |
| First Contentful Paint (FCP)   | **0.7 s** |
| Largest Contentful Paint (LCP) | **0.7 s** |
| Total Blocking Time (TBT)      |  **0 ms** |
| Cumulative Layout Shift (CLS)  | **0.001** |
| Speed Index                    | **0.7 s** |

These results indicate that the website loads quickly, has very low blocking time, and maintains a stable layout.

---

# 🔍 Performance Analysis

## Google Fonts

The main Lighthouse optimization opportunity was related to render-blocking Google Fonts.

The test identified approximately:

**Estimated savings: 490 ms**

The website uses:

* Inter
* JetBrains Mono
* Space Grotesk

The total third-party font payload was approximately **104 KiB**.

Google Fonts was the primary remaining performance optimization opportunity.

However, the actual measured FCP and LCP were already **0.7 seconds**, with **0 ms Total Blocking Time**, so the website demonstrates excellent real loading performance in the Lighthouse desktop test.

---

# ♿ Accessibility Testing

The accessibility score was:

**95/100**

The primary automated issue identified was **color contrast**.

The affected elements included:

```text
.section-label
body text
```

The recommended improvement is to increase the contrast between foreground text and the background.

For normal text, the target should generally meet:

```text
WCAG AA
Contrast Ratio: 4.5:1 or higher
```

For large text:

```text
Contrast Ratio: 3:1 or higher
```

---

# 🔐 Best Practices

The website achieved:

**100/100**

This indicates that the tested implementation passed the Lighthouse best-practice checks.

The project also avoids unnecessary JavaScript execution and maintains a lightweight front-end implementation.

---

# 🔎 SEO

The website achieved:

**100/100**

SEO checks passed for the main page structure.

Important SEO elements include:

* Page title
* Descriptive content
* Proper heading structure
* Link names
* Mobile viewport configuration
* Language declaration
* Search-engine-friendly structure

---

# 🤖 Agentic Browsing

The portfolio achieved:

**2/2**

for the tested agentic browsing checks.

This demonstrates that the website exposes content in a way that automated/agentic browsing can successfully interact with.

---

# 📱 Responsive Design

The portfolio is designed to work across different screen sizes, including:

* Desktop
* Laptop
* Tablet
* Mobile devices

The interface uses modern responsive CSS techniques to maintain usability across screen sizes.

---

# 🚀 Deployment

The portfolio is deployed using **Netlify**.

### Deployment Flow

```text
Local Development
       ↓
     Git
       ↓
    GitHub
       ↓
    Netlify
       ↓
 Live Portfolio
```

Changes pushed to the GitHub repository can be deployed through the connected Netlify deployment workflow.

---

# 🧪 Testing Process

The website was tested using:

1. Google PageSpeed Insights
2. Lighthouse
3. Desktop performance testing
4. Accessibility checks
5. SEO checks
6. Best-practice checks
7. Agentic browsing checks

---

# 📈 Final Evaluation

The final Lighthouse evaluation demonstrates that the portfolio is highly optimized.

### Overall Summary

```text
Performance       ███████████████████▉ 99/100
Accessibility     ███████████████████  95/100
Best Practices    ████████████████████ 100/100
SEO               ████████████████████ 100/100
Agentic Browsing  ████████████████████ 2/2
```

The most important measured performance indicators are excellent:

```text
FCP  → 0.7 s
LCP  → 0.7 s
TBT  → 0 ms
CLS  → 0.001
```

---

# 🔧 Future Improvements

The following improvements can be implemented in future versions:

### 1. Improve Accessibility

Increase the contrast of low-contrast text and verify the result using Lighthouse and accessibility testing tools.

### 2. Optimize Fonts

Possible improvements include:

* Self-hosting required fonts
* Reducing font weights
* Removing unused font families
* Using system fonts where appropriate
* Continuing to use `font-display: swap`

### 3. Improve AI Agent

Future versions could include:

* Larger knowledge base
* Better natural-language understanding
* Intent classification
* Conversation history
* LLM/API integration
* Project-specific question answering

### 4. Add More Projects

The portfolio can be expanded with additional:

* AI/ML projects
* Full-stack projects
* Data science projects
* Automation projects
* Intelligent-agent projects

---

# 📚 Learning Outcomes

Through this project, I gained practical experience in:

* Front-end web development
* Responsive UI design
* JavaScript programming
* AI/ML concepts
* Conversational agents
* Git and GitHub
* Netlify deployment
* Performance optimization
* Lighthouse testing
* Accessibility testing
* SEO optimization
* Agentic web interaction

---

# 🏆 Project Status

**Status: Completed ✅**

The portfolio is deployed and publicly accessible.

### Final Test Status

* [x] Website deployed
* [x] GitHub repository maintained
* [x] Responsive interface
* [x] Interactive AI agent
* [x] Resume download
* [x] Performance tested
* [x] Accessibility tested
* [x] SEO tested
* [x] Best practices tested
* [x] Agentic browsing tested

---

# 📌 Final Project Links

**Live Portfolio:**
https://vasi-portfolio2.netlify.app/

**GitHub:**
https://github.com/vasisaifi1-creator/project1

**LinkedIn:**
https://www.linkedin.com/in/mohdvasisaifi

---

# 👨‍🎓 Student Information

**Name:** Mohd Vasi Saifi
**Program:** B.Tech (Hons.) in Artificial Intelligence & Machine Learning
**University:** SDGI Global University, Ghaziabad
**Expected Graduation:** 2028

---

## ⭐ Conclusion

This project represents my practical application of software engineering, artificial intelligence, web development, and deployment skills.

The final portfolio demonstrates strong performance, excellent SEO and best-practice scores, responsive design, and an interactive AI-powered portfolio experience.

**Final Lighthouse Performance: 99/100**

**Final Lighthouse Accessibility: 95/100**

**Final Lighthouse Best Practices: 100/100**

**Final Lighthouse SEO: 100/100**

**Agentic Browsing: 2/2**

---

**Built with HTML, CSS, JavaScript, AI concepts, GitHub and Netlify.**

**Mohd Vasi Saifi — AI & Software Engineering**

