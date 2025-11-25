# AI-Marketing Crew - Autonomous Marketing Workflow Powered by CrewAI Gemini
Autonomous Marketing Workflow Powered by CrewAI + Gemini

This project builds a fully automated AI Marketing Team using CrewAI and Gemini 2.0 Flash, capable of performing market research, building a marketing strategy, creating a content calendar, drafting social media posts, writing blogs, preparing reel scripts, and optimizing blog articles for SEO.

It turns a collection of specialized AI agents into a coordinated, sequential marketing workflow saving hours of manual work.


# What is CrewAI?

**CrewAI** is an open-source framework for building multi agent AI systems where multiple specialized agents collaborate to perform complex tasks just like a real team.
Link to the documentation: https://docs.crewai.com/

CrewAI enables:

### Multi-Agent Collaboration

Each agent has:

* A role (Head of Marketing, Writer, SEO Specialist…)
* A goal
* A backstory
* Access to tools
* Its own LLM
* Delegation and reasoning abilities

### Task-Based Orchestration

CrewAI structures work into **tasks** and lets agents execute them in:

* Sequential workflows
* Hierarchical workflows
* Parallel workflows

### Built-In Tool Support

Agents can use:

* Web search
* Web scraping
* File reading/writing
* Directory tools
* Browsers
* Custom tools you define

### LLM Flexibility

CrewAI supports:

* Google Gemini
* OpenAI GPT
* Anthropic Claude
* Local LLMs via Ollama
* Azure OpenAI
* Mistral, Groq, etc.

### Perfect for Real World Workflows

CrewAI is ideal for:

* Marketing automation
* Research
* Data analysis
* Content creation
* Software development workflows
* Report generation
* Business operations

---

# Project Overview

This project uses **four AI agents**:

### **1. Head of Marketing**

* Runs market research
* Creates the marketing strategy

### **2. Social Media Content Creator**

* Creates content calendar
* Generates social media posts
* Writes reel scripts

### **3. Blog Content Writer**

* Performs blog topic research
* Writes long-form blogs

### **4. SEO Specialist**

* Optimizes blogs
* Adds metadata, keywords, internal links

The workflow is **fully automated** and runs in a **sequential CrewAI process**.

---

# How the Workflow Runs

### Market Research

The Head of Marketing analyzes:

* Competitors
* Market trends
* Customer needs
* Opportunities

### Marketing Strategy

Creates:

* Messaging
* Positioning
* Budget usage
* Weekly plan (blogs, reels, posts)

### Content Calendar

Outlines:

* Topics
* Formats
* Posting schedule

### Social Media Drafts

Creates post drafts for:

* LinkedIn
* Instagram
* Twitter
* Email campaigns

### Reel Scripts

Creates 15–30 sec scripts with:

* Hooks
* Key message

### Blog Research & Drafting

Performs keyword research and writes structured blogs.

### SEO Optimization

Optimizes blog files with:

* Meta descriptions
* Headings
* Internal links
* Keyword placement

All output files are saved automatically.

---
### Setup Instructions

### Clone the repository

```bash
git clone https://github.com/Subitha-Murugesan/AI-Marketing-Crew-Autonomous-Marketing-Workflow-Powered-by-CrewAI-Gemini.git
cd <repo>
```

### Create virtual environment

```bash
python -m venv venv
source venv/bin/activate 
```

### Add environment variables

Create a `.env` file:

```
SERPER_API_KEY=your_key
GOOGLE_API_KEY=your_key
```

---

# Running the Marketing Crew

Run:

```bash
python crew.py
```

It uses default inputs:

```python
inputs = {
    "product_name": "AI Powered Excel Automation Tool",
    "target_audience": "Small and Medium Enterprises (SMEs)",
    "product_description": "A tool that automates repetitive tasks in Excel using AI, saving time and reducing errors.",
    "budget": "Rs. 50,000",
    "current_date": "YYYY-MM-DD",
}
```


---

# Generated Outputs

After running, you will find:

### Market Research

`resources/drafts/market_research.md`

### Marketing Strategy

`resources/drafts/marketing_strategy.md`

### Content Calendar

`resources/drafts/content_calendar.md`

### Social Media Posts

`resources/drafts/posts/*.md`

### Reel Scripts

`resources/drafts/reels/*.md`

### Blog Drafts

`resources/drafts/blogs/*.md`

### SEO-Optimized Blogs

Output includes:

* Updated titles
* SEO keywords
* Metadata
* Improved structure

---

# Configuration

### Agents - `config/agents.yaml`

Example:

```yaml
head_of_marketing:
  llm: gemini/gemini-2.0-flash
  role: Head of Marketing
  goal: Lead the marketing team...
  backstory: You are an experienced marketing professional...
```

### Tasks - `config/tasks.yaml`

Each task defines:

* Description
* Expected output
* Where to save files
* How agents should handle data

---
## output
<img width="1396" height="430" alt="image" src="https://github.com/user-attachments/assets/5da18ee1-3c6e-48b8-9490-b56e8844b50e" />
<img width="1418" height="589" alt="image" src="https://github.com/user-attachments/assets/56a66f06-c7f1-4fe9-ba1c-8b45fe6cfeaa" />


