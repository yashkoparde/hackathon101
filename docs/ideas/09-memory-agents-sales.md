---
title: Memory Agents - Sales & Revenue
author: yashkoaprde
part_of: Yash Hackathon Guide
---

# Sales & Revenue Memory Agents

[← Idea Index](00-IDEA-INDEX.md)

## 1. Deal Intelligence Agent

**The Problem:** Sales reps waste hours reading CRM notes before calls. An agent with deal memory can brief a rep in seconds and suggest winning tactics based on past deals.

### System Architecture
```mermaid
flowchart LR
 A[Sales Rep] -->|Queries| B(Frontend Dash)
 B --> C{Backend API}
 C -->|Fetch Context| D[(Vector DB: Past Deals)]
 C -->|Fetch CRM Data| E[(Salesforce API)]
 D & E --> F[LLM Synthesis]
 F --> B
```

### The Demo Execution
```mermaid
sequenceDiagram
 participant Rep
 participant Agent
 participant DB
 Rep->>Agent: "Prep me for Call 4 with Acme Corp"
 Agent->>DB: Retrieve Acme transcripts & metadata
 DB-->>Agent: Objections: Pricing, Security
 Agent-->>Rep: "They will object to price. Counter with ROI case study."
```

**Technical Scope & Anti-Patterns:**
* **Tech Stack:** Next.js, Pinecone (Vector DB), OpenAI API, mock CRM JSON data.
* **Advanced Scope:** Live webhook integration to auto-log objections post-call.
* **Anti-pattern:** Trying to build a live Zoom transcription integration. Stick to static logs.

---

## 2. Outbound Prospecting Agent

**The Problem:** Outbound is a numbers game, but personalization wins. An agent that remembers and adapts its approach across hundreds of prospects is a force multiplier.

### System Architecture
```mermaid
flowchart TD
 A[Prospect Data] --> B(LLM Draft Engine)
 B --> C[Email Batch A]
 C --> D{Response Parser}
 D -->|Bounce/Ignore| E[(Failure Memory)]
 D -->|Reply/Open| F[(Success Memory)]
 E & F --> B
```

### The Demo Execution
```mermaid
sequenceDiagram
 participant User
 participant Agent
 participant Memory
 User->>Agent: "Draft emails for Persona B"
 Agent->>Memory: Check past results for Persona B
 Memory-->>Agent: "Formal tone failed. Short/casual succeeded."
 Agent-->>User: Outputs optimized, casual copy.
```

**Technical Scope & Anti-Patterns:**
* **Tech Stack:** Python FastAPI, LangChain, Postgres for tracking state.
* **Advanced Scope:** Connects to LinkedIn API to fetch live persona data.
* **Anti-pattern:** Building a full email client. Just output the suggested copy.

---

## 3. Proposal & RFP Agent

**The Problem:** RFP responses are time sinks. An agent that remembers your best past answers and tailors them to each new opportunity saves days per proposal.

### System Architecture
```mermaid
flowchart LR
 A[New RFP Question] --> B{Semantic Router}
 B --> C[(Past RFP Vector Store)]
 C --> D[Retrieve Top 3 Matches]
 D --> E[LLM Tailoring]
 E --> F[Final Answer]
```

### The Demo Execution
```mermaid
sequenceDiagram
 participant User
 participant System
 User->>System: Paste RFP security question
 System->>System: Retrieve 2 past winning answers
 System->>System: Synthesize based on new client context
 System-->>User: Returns tailored paragraph + flags conflicting terms
```

**Technical Scope & Anti-Patterns:**
* **Tech Stack:** React, FastAPI, ChromaDB, OpenAI.
* **Advanced Scope:** Flags conflicting SLA terms against past legal commitments.
* **Anti-pattern:** Generating a 50-page PDF. Just generate the raw text answers in the UI.

---
Maintained by [@yashkoaprde](https://github.com/yashkoaprde)
