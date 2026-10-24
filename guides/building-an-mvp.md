# Building an MVP Under Time Constraints

> "An MVP is not a broken, half-finished version of a 10-feature app. It is a complete, polished, working version of one core feature."

In a hackathon, time is your scarcest resource. Teams often run out of time because they try to build login systems, user settings, profile photo uploaders, payment gateways, and dark mode toggles before implementing the actual core intelligence of their product.

---

## 1. What is a Hackathon MVP?

A Minimum Viable Product (MVP) in a hackathon has one job: **to prove your core hypothesis works in front of an audience.**

```
   ┌──────────────────────────────────────────────────────────────┐
   │                       Full Product Vision                    │
   │ [Auth] ── [Profiles] ── [CORE ALGORITHM] ── [Billing] ── ... │
   └────────────────────────────────┬─────────────────────────────┘
                                    │
                                    ▼
                      ┌───────────────────────────┐
                      │      HACKATHON MVP        │
                      │  Mock User ──► [CORE ENGINE]  │
                      └───────────────────────────┘
```

If your project is an AI diagnostic scanner, your MVP is **upload image ➔ run model ➔ display diagnostic report with confidence bounds**. You do NOT need sign-up verification emails, Stripe billing, or password reset tokens.

---

## 2. The Ruthless Scoping Framework

When scoping your prototype, divide your feature wishlist into three buckets:

| Tier | Priority | Examples | Rule |
|---|---|---|---|
| **Tier 1: Core Value Loop** | Essential (P0) | The primary algorithm, transformation, or prediction | **Must work 100% reliably in demo.** |
| **Tier 2: Supporting Polish** | Secondary (P1) | Visual chart, export to PDF, clean toast notifications | Build only if Tier 1 is tested and stable. |
| **Tier 3: Distractions** | Ignored (P2) | Sign up with OAuth, admin dashboards, settings page | **Cut immediately.** Hardcode mock data. |

> **Pro Tip:** If a feature doesn't directly contribute to the judge's "Aha!" moment during a 3-minute pitch, cut it.

---

## 3. Battle-Tested Hackathon Tech Stacks

Choose tools that prioritize development speed, rapid iteration, and reliable zero-config hosting:

```
┌─────────────────────────────────────────────────────────────┐
│                      FRONTEND / UI                          │
│  Next.js (App Router) + Tailwind CSS + shadcn/ui            │
├─────────────────────────────────────────────────────────────┤
│                    BACKEND / BUSINESS LOGIC                 │
│  FastAPI (Python) OR Express/Hono (TypeScript/Node.js)      │
├─────────────────────────────────────────────────────────────┤
│                   STORAGE / DATABASE                        │
│  Supabase (PostgreSQL + instant REST API) OR SQLite / Redis │
├─────────────────────────────────────────────────────────────┤
│                      HOSTING & DEPLOYMENT                   │
│  Vercel (Frontend/Serverless) + Render / Modal (FastAPI/GPU)│
└─────────────────────────────────────────────────────────────┘
```

### Why This Stack Excels:
- **FastAPI / Python:** Direct integration with ML libraries, LangChain, HuggingFace, and iNSIGHTS AI endpoints. Auto-generates interactive Swagger documentation at `/docs`.
- **Next.js & Tailwind & shadcn/ui:** Copy-paste accessible, pre-styled components (buttons, modals, tables, badges) in seconds without designing from scratch.
- **Supabase:** Provides instant relational tables, auth, and real-time triggers without manual schema migrations or server setup.

---

## 4. Preventing "Integration Hell"

The most dangerous phase of a hackathon happens between 1:00 AM and 4:00 AM, when the frontend and backend developers attempt to merge their branches for the first time.

### The Contract-First Protocol

To eliminate integration breakdowns, establish API contracts before writing code:

1. **Agree on JSON Schemas First:**
   Spend 15 minutes defining the exact request and response JSON payloads:
   ```json
   // POST /api/analyze
   // Request:
   { "query": "string", "source_url": "string" }
   
   // Response:
   { "status": "success", "summary": "string", "metrics": { "confidence": 0.94 } }
   ```
2. **Build with Mock Endpoints:**
   The frontend developer uses a local mock JSON response so they can build and polish the UI independently without waiting for the backend to be completed.
3. **Switch the Base URL:**
   Once the backend server is live, flip `NEXT_PUBLIC_API_URL` to point to the live server.

---

## 5. Fallbacks and Hardcoded Safety Nets

Live APIs fail, rate limits get exceeded, and conference Wi-Fi introduces latency. Professional hackathon teams engineer safety nets:

- **Cached Mock Fallback:** If your third-party API or LLM request times out, write a simple try/catch fallback that returns realistic pre-computed data.
- **Deterministic Seed Data:** Pre-populate your database with 5 to 10 rich sample entries so judges never look at empty tables or blank states.
- **Health Check Endpoint:** Include a `/healthz` route to verify connectivity instantly.

---

## 6. MVP Development Schedule (24-Hour Timeline)

```
[00:00 - 02:00]  Problem Definition & API Contract Draft
[02:00 - 08:00]  Core Engine Implementation & UI Scaffolding
[08:00 - 13:00]  Frontend-Backend Integration & Live Testing
[13:00 - 18:00]  Edge Case Handling, Error Boundaries & Polish
[18:00 - 21:00]  Code Freeze, Cloud Deployment & Smoke Test
[21:00 - 24:00]  Slide Deck Finalization & Live Demo Rehearsal
```

---

## 7. Next Steps

- Prepare your demo and presentation: **[Pitching & Demos](pitching-and-demos.md)**
- Use the ready-made spec document: **[MVP Planning Template](../templates/mvp-planning.md)**
