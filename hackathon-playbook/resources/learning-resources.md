# Learning Resources & Documentation

> "The best hackathon developers are not the ones who memorized documentation; they are the ones who can read official docs and deploy a library within 20 minutes."

A curated library of technical tutorials, open-source project examples, and cheat sheets to prepare your team before and during the hackathon.

---

## 1. Technical Framework Tutorials & Quickstarts

### Web & Full-Stack
- **[Learn Next.js Official Tutorial](https://nextjs.org/learn):** Interactive step-by-step introduction to Next.js App Router, Server Components, and client fetching.
- **[FastAPI Comprehensive Guide](https://fastapi.tiangolo.com/tutorial/):** Understand path parameters, Pydantic data schemas, request validation, and CORS handling.
- **[Full Stack Open](https://fullstackopen.com/en/):** Deep dive into modern web development, React, REST APIs, and state management.
- **[Tailwind CSS Screencasts](https://tailwindcss.com/screencasts):** 5-minute visual guides on building responsive grid systems and complex UI layouts.

### AI, ML & LLM Engineering
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

## 3. Hackathon Cheat Sheets

Keep these short references handy:

### Git Hackathon Commands
```bash
# Clone the repository
git clone <repo-url>
cd <repo-name>

# Create and checkout your feature branch
git checkout -b feat/core-api

# Keep in sync with main before pushing
git fetch origin
git merge origin/main

# Stage, commit, and push
git add .
git commit -m "feat(api): implement mock inference endpoint"
git push origin feat/core-api
```

### Environment Variable Checklist
Create a `.env.example` file in your repository root with dummy placeholder keys:
```env
NEXT_PUBLIC_API_URL=http://localhost:8000
DATABASE_URL=postgresql://user:password@localhost:5432/mydb
INSIGHTS_AI_API_KEY=your_insights_ai_key_here
GROQ_API_KEY=your_groq_api_key_here
```
> **Warning:** Never commit `.env` containing live secrets or credentials to public Git repositories.

---

## 4. Next Steps

- Explore iNSIGHTS AI capabilities: **[iNSIGHTS AI Deep Dive](insights-ai.md)**
- Review operational rules: **[Rules & Guidelines](../mini-hackathon/rules-and-guidelines.md)**
