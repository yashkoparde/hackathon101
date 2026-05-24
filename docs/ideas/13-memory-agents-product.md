---
title: Memory Agents - Product & Strategy
author: yashkoaprde
part_of: Yash Hackathon Guide
---

# Product & Strategy Memory Agents

[← Idea Index](00-IDEA-INDEX.md)

## 1. User Feedback Synthesizer

**The Problem:** Product teams drown in feedback. An agent that connects dots across channels and time spots patterns humans miss.

### System Architecture
```mermaid
flowchart LR
 A[Intercom] --> C
 B[Twitter] --> C
 C{Ingestion Pipeline} --> D[(Time-Series DB)]
 D --> E[Sentiment & Theme Engine]
 E --> F[Product Dashboard]
```

### The Demo Execution
```mermaid
sequenceDiagram
 participant PM
 participant Agent
 participant DB
 PM->>Agent: "What's our top churn risk?"
 Agent->>DB: Scan 6 months of Intercom + Twitter
 Agent-->>PM: "Theme 'Slow API' spiked 40% in Q3. Here are 50 quotes grouped by severity."
```

**Technical Scope & Anti-Patterns:**
* **Tech Stack:** React, Python, InfluxDB or TimescaleDB.
* **Advanced Scope:** Agent automatically drafts a PRD (Product Requirements Document) for the most requested feature.
* **Anti-pattern:** Building a simple summarizer. It must track *shifts over time* to prove memory.

---

## 2. Competitive Intelligence Agent

**The Problem:** Competitive intelligence is only useful if it is cumulative. An agent that remembers six months of competitor activity spots patterns a weekly check never would.

### System Architecture
```mermaid
flowchart TD
 A[Pricing Pages] --> C
 B[Job Boards] --> C
 C{Web Scraper} --> D[(Snapshot Memory)]
 D --> E[Pattern Recognizer]
 E --> F[Intel Report]
```

### The Demo Execution
```mermaid
sequenceDiagram
 participant User
 participant Agent
 User->>Agent: "What is Competitor X planning?"
 Agent->>Agent: Cross-reference 6 months of snapshots
 Agent-->>User: "They hired 5 AI engineers in May and changed their pricing structure yesterday. Expect an AI tier launch."
```

**Technical Scope & Anti-Patterns:**
* **Tech Stack:** Node.js, Puppeteer/Cheerio, Postgres JSONb.
* **Advanced Scope:** Scrapes live competitor subreddits to cross-reference customer complaints with their feature releases.
* **Anti-pattern:** Building a web scraper. The value is the historical synthesis, not the scraping.

---

## 3. Meeting Prep Agent

**The Problem:** An agent that briefs you with full context from every past interaction with a contact is a professional superpower.

### System Architecture
```mermaid
flowchart LR
 A[Calendar Invite] --> B{Agent Gateway}
 B --> C[(Past Transcripts DB)]
 C --> D[Extract Promises/Misses]
 D --> E[1-Pager Synthesis]
 E --> F[Email to User]
```

### The Demo Execution
```mermaid
sequenceDiagram
 participant User
 participant Agent
 participant DB
 User->>Agent: "Prep me for John Doe."
 Agent->>DB: Fetch Q1 and Q2 meeting transcripts
 Agent-->>User: "In Q2, you promised him the API docs. He missed the Q1 follow-up. Ask about his new Series A funding."
```

**Technical Scope & Anti-Patterns:**
* **Tech Stack:** Vue.js, FastAPI, ChromaDB, Google Calendar API.
* **Advanced Scope:** Integrates with Zoom transcript APIs to automatically append new promises post-meeting.
* **Anti-pattern:** Building a generic meeting transcriber. The wow factor is the pre-meeting historical recall.

---
Maintained by [@yashkoaprde](https://github.com/yashkoaprde)
