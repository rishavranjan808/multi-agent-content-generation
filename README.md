# Agentic AI Research Assistant

A multi-agent AI system built using **CrewAI**, **OpenAI GPT-4**, and **YouTube Knowledge Extraction Tools** to automate research and content creation. The application uses specialised AI agents to analyse educational YouTube content, extract key insights, and generate high-quality technical articles on AI, Machine Learning, Data Science, and related topics.

---

## Project Overview

Traditional content creation requires significant time for research, information gathering, fact verification, and writing. This project demonstrates how autonomous AI agents can collaborate to streamline that process.

The system leverages CrewAI's multi-agent orchestration framework to assign specialised responsibilities to separate AI agents:

- A **Research Agent** gathers and analyses relevant information from YouTube educational content.
- A **Writer Agent** transforms research findings into structured and engaging technical articles.

By combining autonomous agents with external knowledge retrieval, the system simulates a collaborative AI research and writing workflow.

---

## Features

### Multi-Agent Architecture

The application uses multiple specialised AI agents that collaborate to complete complex tasks.

#### Research Agent

Responsible for:

- Searching educational YouTube content
- Extracting relevant information
- Identifying key concepts
- Gathering supporting knowledge for the topic

#### Writer Agent

Responsible for:

- Organising research findings
- Generating structured content
- Creating readable technical articles
- Simplifying complex concepts

---

### YouTube Knowledge Extraction

Utilises CrewAI's YouTube search capabilities to retrieve topic-specific information from educational content.

Current implementation searches content from:

```text
@krishnaik06
```

---

### Autonomous Task Orchestration

CrewAI coordinates agent collaboration using a sequential workflow:

```text
Research Agent
        ↓
Research Output
        ↓
Writer Agent
        ↓
Final Blog Article
```

---

### Agent Memory

Agents maintain contextual memory throughout execution, enabling better continuity and improved content generation.

---

### Caching Support

The application uses CrewAI caching mechanisms to improve performance and reduce repeated processing.

---

## System Architecture

```text
User Topic
     │
     ▼
Research Task
     │
     ▼
Blog Researcher Agent
     │
     ▼
YouTube Search Tool
     │
     ▼
Knowledge Extraction
     │
     ▼
Blog Writer Agent
     │
     ▼
Content Generation
     │
     ▼
Final Article
```

---

## Technology Stack

### AI & LLM

- OpenAI GPT-4
- CrewAI

### Agent Framework

- CrewAI Agents
- CrewAI Tasks
- CrewAI Process Management

### Knowledge Retrieval

- YouTube Channel Search Tool
- External Content Analysis

### Backend

- Python

### Environment Management

- Python Dotenv

---

## Project Structure

```text
.
├── agents.py          # AI agent definitions
├── tasks.py           # Task definitions
├── tools.py           # YouTube search tools
├── crew.py            # Crew orchestration logic
├── requirements.txt   # Project dependencies
└── README.md
```

---

## Agents

### Blog Researcher Agent

**Role:** Blog Researcher from YouTube Videos

Responsibilities:

- Search relevant videos
- Analyse educational content
- Extract useful information
- Provide structured insights

Capabilities:

- Memory enabled
- Tool access enabled
- Delegation enabled

---

### Blog Writer Agent

**Role:** Blog Writer

Responsibilities:

- Convert research into written content
- Generate engaging articles
- Simplify technical concepts
- Improve readability

Capabilities:

- Memory enabled
- Access to research output
- Content generation

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/agentic-ai-research-assistant.git

cd agentic-ai-research-assistant
```

---

### Create Virtual Environment

```bash
python -m venv venv
```

Linux/macOS

```bash
source venv/bin/activate
```

Windows

```bash
venv\Scripts\activate
```

---

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

### Configure Environment Variables

Create a `.env` file:

```env
OPENAI_API_KEY=YOUR_API_KEY
```

---

### Run the Project

```bash
python crew.py
```

---

## Example Usage

Input:

```text
AI VS ML VS DL vs Data Science
```

Output:

```text
A comprehensive article explaining:

- Artificial Intelligence
- Machine Learning
- Deep Learning
- Data Science

Including relationships, differences,
real-world applications, and examples.
```

---

## Use Cases

- AI Research Automation
- Technical Content Generation
- Educational Blog Creation
- Knowledge Extraction from YouTube
- Learning Material Generation
- Research Summarisation
- Agentic AI Experimentation

---

## Key Concepts Demonstrated

### Agentic AI

Implementation of autonomous AI agents with specialised responsibilities.

### Multi-Agent Systems

Collaboration between independent agents to solve complex tasks.

### Tool Calling

Integration of external tools within autonomous agent workflows.

### LLM Orchestration

Management of multiple AI agents using CrewAI.

### Knowledge Augmentation

Enhancing LLM outputs through external information retrieval.

---

## Future Enhancements

- Support for multiple YouTube channels
- Dynamic channel selection
- Web search integration
- RAG-based knowledge retrieval
- Streamlit web interface
- PDF export functionality
- LinkedIn post generation
- Newsletter creation
- Multi-language support

---

## Limitations

- Currently configured for a specific YouTube channel.
- Requires an OpenAI API key.
- Output quality depends on source content availability.
- Internet connection required for knowledge retrieval.

---

## Learning Outcomes

This project demonstrates practical experience with:

- CrewAI
- LLM Orchestration
- Multi-Agent Systems
- Autonomous Agents
- Tool Integration
- Prompt Engineering
- OpenAI APIs
- Agent Memory and Task Planning

---

## Disclaimer

This project is intended for educational and research purposes. Generated content should be reviewed for accuracy before publication or professional use.

---

⭐ If you find this project useful, consider giving the repository a star.
