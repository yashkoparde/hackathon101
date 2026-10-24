# Learning Resources & Documentation

> "The best hackathon developers are not the ones who memorized documentation; they are the ones who can read official docs and deploy a library within 20 minutes."

A curated library of technical tutorials, open-source project examples, and cheat sheets to prepare your team before and during the hackathon sprint on **31 October 2026**.

---

## 1. Technical Framework Tutorials & Quickstarts

### Web & Full-Stack
- **[Learn Next.js Official Tutorial](https://nextjs.org/learn):** Interactive step-by-step introduction to Next.js App Router, Server Components, and client fetching.
- **[FastAPI Comprehensive Guide](https://fastapi.tiangolo.com/tutorial/):** Understand path parameters, Pydantic data schemas, request validation, and CORS handling.
- **[Full Stack Open](https://fullstackopen.com/en/):** Deep dive into modern web development, React, REST APIs, and state management.
- **[Tailwind CSS Screencasts](https://tailwindcss.com/screencasts):** 5-minute visual guides on building responsive grid systems and complex UI layouts.

### AI, ML & LLM Engineering
- **[iNSIGHTS AI Documentation](https://insights-ai.info):** Explore Deep Search, Document Intelligence, and PredictX tool capabilities.
- **[LangChain Official Documentation](https://python.langchain.com/docs/get_started/introduction):** Quickstarts for building agentic chains, memory buffers, and retrieval-augmented generation (RAG).
- **[Hugging Face NLP Course](https://huggingface.co/learn/nlp-course):** Practical transformer workflows, tokenizers, and model fine-tuning.
- **[Pinecone Vector Database Architecture Guide](https://www.pinecone.io/learn/):** Semantic search patterns and vector indexing fundamentals.

---

## 2. Public Repositories & Blueprint Codebases

Studying how winning projects structure their code is the fastest way to improve:

| Repository / Blueprint | Core Concept | What You Can Learn |
|---|---|---|
| **[shadcn/taxonomy](https://github.com/shadcn-ui/taxonomy)** | Full-stack Next.js web application | Authentication, Prisma schema, Tailwind UI patterns, and clean server actions |
| **[tiangolo/full-stack-fastapi-template](https://github.com/tiangolo/full-stack-fastapi-template)** | Python FastAPI + React + PostgreSQL | Complete Docker setup, JWT authentication, and background worker queues |
| **[langchain-ai/rag-from-scratch](https://github.com/langchain-ai/rag-from-scratch)** | Multi-stage Retrieval Augmented Generation | Document chunking, vector embedding, and hallucination reduction techniques |

---

## 3. Team Git Collaboration Workflow

To avoid merge conflicts at 2:00 PM, follow this team branching model:

```mermaid
gitGraph
    commit id: "Initial Repo Setup"
    branch feat/api-backend
    checkout feat/api-backend
    commit id: "FastAPI schema skeleton"
    commit id: "Connect iNSIGHTS AI"
    checkout main
    branch feat/frontend-ui
    checkout feat/frontend-ui
    commit id: "Tailwind & shadcn cards"
    commit id: "Wire mock response"
    checkout main
    merge feat/api-backend id: "Merge Backend (12:30 PM)"
    checkout feat/frontend-ui
    merge main id: "Sync Main into Frontend"
    commit id: "Flip API URL to live"
    checkout main
    merge feat/frontend-ui id: "End-to-End Ready (02:00 PM)"
    commit id: "Final Code Freeze & README (02:45 PM)" tag: "v1.0-submission"
```

### Git Terminal Cheat Sheet
```bash
# 1. Clone the team repository
git clone https://github.com/your-team/hackathon-mvp.git
cd hackathon-mvp

# 2. Create your isolated feature branch
git checkout -b feat/hero-flow

# 3. Pull latest changes from main before committing
git fetch origin
git merge origin/main

# 4. Stage, commit with conventional message, and push
git add .
git commit -m "feat(api): implement document parsing route"
git push origin feat/hero-flow
```

---

## 4. Environment Variables Checklist

Create a `.env.example` file in your repository root with dummy placeholder keys:
```env
NEXT_PUBLIC_API_URL=http://localhost:8000
DATABASE_URL=postgresql://user:password@localhost:5432/mydb
INSIGHTS_AI_API_KEY=your_insights_ai_key_here
GROQ_API_KEY=your_groq_api_key_here
```

> [!CAUTION]
> **Never commit your `.env` file containing live secrets or private tokens to public Git repositories.** Add `.env` to `.gitignore` immediately upon project creation.

---

## 5. Next Steps

- Explore iNSIGHTS AI platform details: **[iNSIGHTS AI Guide](insights-ai.md)**
- Review operational rules: **[Rules & Guidelines](../mini-hackathon/rules-and-guidelines.md)**
