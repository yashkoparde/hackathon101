---
title: Tech Stack Cheatsheet
author: yashkoaprde
part_of: Yash Hackathon Guide
---

# Tech Stack Cheatsheet

[← Back to README](../README.md) · [← Demo Playbook](04-DEMO-PLAYBOOK.md)

Fast, boring, reliable defaults by project type. The goal in a hackathon is *speed to a working demo*, not the most impressive architecture.

## General Principle

> [!TIP]
> Optimize for "what can we ship working code in fastest," not "what looks best on a resume." 

If nobody on your team knows Kubernetes, do not try to learn Kubernetes at 2 AM on a Saturday. Just use Vercel.

---

## By Project Type

### Web App (The Safest Default)
- **Frontend:** React/Next.js, or plain HTML/CSS/JS if the UI is simple.
- **Styling:** Tailwind CSS + shadcn/ui or Radix. You don't have time to write raw CSS grids.
- **Backend:** Node/Express or Python/FastAPI. Pick whichever your team can write without looking up docs.
- **Database:** Supabase (Postgres) or Firebase. Do not install a database locally unless you want to lose 3 hours to Docker bugs.
- **Auth:** Skip it. Hardcode a fake user profile. If you *must* have auth, use Clerk.
- **Hosting:** Vercel (Frontend) + Render/Railway (Backend). 

### AI / LLM-Powered Projects
- **LLM access:** Use whatever API gives you free credits. OpenAI is the easiest.
- **Orchestration:** Direct API calls. Do not use LangChain or heavy agent frameworks unless you already know them. They add unnecessary complexity for a weekend project.
- **Vector search:** Supabase pgvector or Pinecone.
- **Structured output:** Prompt for JSON explicitly and validate defensively. LLMs occasionally add stray markdown text around JSON.

### Mobile
- **Cross-platform:** React Native (Expo) or Flutter.
- **Fastest path:** A responsive web app that *looks* like an app (add-to-homescreen, mobile-first design) is usually faster to demo well than a real native build in 36 hours.

### Data / Dashboard Projects
- **Quick charts:** Recharts, Tremor, or Chart.js.
- **No-backend option:** Static site + client-side data processing (Papaparse for CSV).
- **Notebook-to-demo:** If your core work is analysis, build a clean Streamlit app instead of a custom frontend.

### Hardware / IoT
- **Prototype fast:** Simulate sensor input in software first. Wire up real hardware only once the logic works.
- **Demo risk:** Hardware demos fail live. **Always** have a recorded backup ready.

---

## The "Do Not Do This" List

- Setting up CI/CD pipelines, Docker orchestration, or Kubernetes.
- Building your own auth system from scratch.
- Microservices. One monolithic app is faster and more reliable to demo.
- Picking a database you need to learn from scratch.
- Perfecting responsive design. Optimize for the exact screen you will present on.

---

## Quick Decision Matrix

| If your core value is... | Default to... |
|---|---|
| A user-facing app | Next.js + Tailwind + Supabase |
| An AI capability | Direct OpenAI API calls + FastAPI |
| A dataset/insight | Streamlit or Next.js + Tremor |
| A physical interaction | Software simulation first, Arduino second |

---
Maintained by [@yashkoaprde](https://github.com/yashkoaprde) · [Next: Common Mistakes →](06-COMMON-MISTAKES.md)
