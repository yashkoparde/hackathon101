---
title: AI & Agents
author: yashkoaprde
part_of: Yash Hackathon Guide
---

# AI & Agents

[← Back to Idea Index](00-IDEA-INDEX.md) · [← Productivity Tools](01-productivity-tools.md)

Stateless chatbots are yesterday's news. The frontier is **agents with memory** : systems that learn from past interactions, adapt to user behavior, and compound in value over time.

Do not build a generic "AI tutor" or "AI quiz generator." Build something that solves a brutal, unglamorous business problem where *remembering context* is the entire value proposition.

| Idea | Problem | MVP Demo | Advanced Scope | Anti-pattern |
|---|---|---|---|---|
| **The Deal Intelligence Agent (Sales)** | Enterprise sales reps waste hours re-reading CRM notes before every client call. They forget specific objections raised 3 months ago or pricing concerns mentioned by a junior stakeholder. | 1. Ingest 3 transcripts from past sales calls. | | Do not try to build a real-time Zoom integration. Upload static text transcripts. |
| **The Content Strategy Agent (Marketing)** | Marketing teams constantly reinvent the wheel. They forget what performed well last year, repeat topics, and lose track of their brand voice. | 1. Feed the agent the titles and performance metrics of 20 past blog posts. | | Do not have the agent actually write the 2,000-word post. Generate the *strategy* and the *outline*. |
| **The Competitive Intelligence Agent (Product)** | Product managers try to track competitor moves (pricing changes, feature launches, hiring patterns), but the data is scattered and cumulative context is lost. | 1. Scrape a competitor's changelog or pricing page across 3 different dates (use the Wayback Machine for source data). | | Do not build a live web scraper. Feed it hardcoded Markdown dumps of web pages to ensure the demo never fails. |
| **The Meeting Prep Agent (Executive Ops)** | Executives have 12 meetings a day. They cannot remember what they promised a specific vendor during a passing conversation 4 weeks ago. | 1. Store simulated email threads and meeting notes for 5 different contacts. | | Do not integrate with Google Calendar APIs. Hardcode the "upcoming meeting" trigger. |

---
Maintained by [@yashkoaprde](https://github.com/yashkoaprde)
