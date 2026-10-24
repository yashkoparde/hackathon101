# The Hackathon101
 
</div>

<br />

A highly opinionated playbook for shipping hackathon projects that don't suck. I cover how to select a stack, build the core logic in a weekend, and demo it without it crashing. Use it for any hackathon, any tech stack, any sponsor.

No bs. No theory. Just engineering pragmatism. Here is how you survive a 48-hour sprint without losing your mind or burning out.

---

## The Engineering Lifecycle

This is the exact timeline you need to follow if you actually want to ship working code:

<details>
<summary><b>Click to expand the 48-Hour Sprint Timeline</b></summary>
<br>

```mermaid
gantt
 title The 48-Hour Hackathon Sprint
 dateFormat YYYY-MM-DD HH:mm
 axisFormat %H:%M
 
 section Friday Night
 Ideation & Scoping :crit, a1, 2024-01-05 18:00, 3h
 Wireframing & Stack Setup:active, a2, after a1, 3h
 Sleep (Mandatory) :done, a3, after a2, 6h

 section Saturday
 Core Logic & APIs :active, b1, 2024-01-06 06:00, 8h
 Frontend Skeleton :active, b2, after b1, 6h
 Integration Hell :crit, b3, after b2, 4h
 Sleep (Mandatory) :done, b4, after b3, 6h

 section Sunday
 Cut Scope & Hardcode :crit, c1, 2024-01-07 06:00, 3h
 Demo Polish & Rehearsal :crit, c2, after c1, 3h
 Pencils Down & Pitch :active, c3, after c2, 2h
```

</details>

---

## 🏆 INVICTUS Hackathons Playbook

The official **INVICTUS Hackathons Playbook** (invictus-hackathons-playbook/) — student guides, rapid MVP engineering frameworks, [iNSIGHTS AI](https://insights-ai.info) research workflows, and the turnkey operating manual for INVICTUS mini hackathons.

👉 **[Explore the full INVICTUS Hackathons Playbook ➔](invictus-hackathons-playbook/README.md)**

`
invictus-hackathons-playbook/
├── guides/               # Core student curriculum & methodology
│   ├── what-are-hackathons.md
│   ├── finding-hackathons.md
│   ├── research-and-ideation.md
│   ├── building-an-mvp.md
│   └── pitching-and-demos.md
├── resources/            # Tools, platforms, and iNSIGHTS AI integration
│   ├── tools-and-platforms.md
│   ├── learning-resources.md
│   └── insights-ai.md
├── mini-hackathon/       # Operational manual for hosting events
│   ├── event-overview.md
│   ├── rules-and-guidelines.md
│   ├── timeline.md
│   ├── judging-criteria.md
│   ├── submission-guidelines.md
│   └── organizer-checklist.md
└── templates/            # Ready-to-use markdown templates
    ├── problem-statement.md
    ├── mvp-planning.md
    ├── pitch-deck.md
    ├── project-readme.md
    └── judging-scorecard.md
`

### 📂 Playbook Directory Index

#### 📘 [1. Guides (guides/)](invictus-hackathons-playbook/guides/)
- 📄 [**what-are-hackathons.md**](invictus-hackathons-playbook/guides/what-are-hackathons.md) — What hackathons are, formats (software, AI, civic tech), myths vs reality, beginner tips.
- 📄 [**finding-hackathons.md**](invictus-hackathons-playbook/guides/finding-hackathons.md) — Discovery platforms (Devfolio, Unstop, Devpost), evaluation matrix, team formation.
- 📄 [**research-and-ideation.md**](invictus-hackathons-playbook/guides/research-and-ideation.md) — Dissecting problem statements, market gaps, target users, research with iNSIGHTS AI.
- 📄 [**building-an-mvp.md**](invictus-hackathons-playbook/guides/building-an-mvp.md) — The Ruthless Scoping Rule, tech stacks (Next.js, FastAPI, Supabase), API contracts.
- 📄 [**pitching-and-demos.md**](invictus-hackathons-playbook/guides/pitching-and-demos.md) — The 3-minute pitch formula, live demo defense, judge Q&A, post-hackathon journey.

#### 🛠️ [2. Resources & AI (
esources/)](invictus-hackathons-playbook/resources/)
- 📄 [**tools-and-platforms.md**](invictus-hackathons-playbook/resources/tools-and-platforms.md) — UI libraries (shadcn/ui, Tailwind), BaaS (Supabase, Neon), AI APIs (Groq, HF), hosting (Vercel).
- 📄 [**learning-resources.md**](invictus-hackathons-playbook/resources/learning-resources.md) — Framework tutorials, open-source repos to study, Git commands, .env.example setup.
- 📄 [**insights-ai.md**](invictus-hackathons-playbook/resources/insights-ai.md) — Deep dive into [insights-ai.info](https://insights-ai.info): Deep Search, Document Intelligence, PredictX.

#### ⚡ [3. Mini Hackathon Operating Manual (mini-hackathon/)](invictus-hackathons-playbook/mini-hackathon/)
- 📄 [**event-overview.md**](invictus-hackathons-playbook/mini-hackathon/event-overview.md) — Purpose, first-year focus, eligibility, team size, themes, and 5-phase structure.
- 📄 [**rules-and-guidelines.md**](invictus-hackathons-playbook/mini-hackathon/rules-and-guidelines.md) — Original code policy, permissible boilerplates, AI ethics, disqualification rules.
- 📄 [**timeline.md**](invictus-hackathons-playbook/mini-hackathon/timeline.md) — 6-Hour Express Schedule, 24-Hour Hackathon Timeline, hour-by-hour milestone checklist.
- 📄 [**judging-criteria.md**](invictus-hackathons-playbook/mini-hackathon/judging-criteria.md) — 100-point rubric (Relevance 25, Prototype 30, Innovation 20, Demo 15, Learning 10).
- 📄 [**submission-guidelines.md**](invictus-hackathons-playbook/mini-hackathon/submission-guidelines.md) — Mandatory deliverables (Repo, README, Live MVP, Slides, Demo Video) & late policy.
- 📄 [**organizer-checklist.md**](invictus-hackathons-playbook/mini-hackathon/organizer-checklist.md) — Step-by-step checklist for pre-event, venue AV/power, sprint execution, and awards.

#### 📋 [4. Field Templates (	emplates/)](invictus-hackathons-playbook/templates/)
- 📄 [**problem-statement.md**](invictus-hackathons-playbook/templates/problem-statement.md) — Problem Statement Analysis, User Persona, Competitor Gap Matrix, Validation log.
- 📄 [**mvp-planning.md**](invictus-hackathons-playbook/templates/mvp-planning.md) — Single core user flow spec, Tier 1/2/3 scope cuts, API request/response contracts.
- 📄 [**pitch-deck.md**](invictus-hackathons-playbook/templates/pitch-deck.md) — 7-slide pitch deck structure with speaking cues and time splits (180 seconds).
- 📄 [**project-readme.md**](invictus-hackathons-playbook/templates/project-readme.md) — Production-grade GitHub README boilerplate with setup guides and architecture block.
- 📄 [**judging-scorecard.md**](invictus-hackathons-playbook/templates/judging-scorecard.md) — Official printable/digital judging sheet with rubric weights and feedback sections.

---

## Interactive Playbook Directory

<details open>
<summary><b>Click to explore the playbook</b></summary>
<br>

### Core Strategy Guides
| Guide | What it covers |
|---|---|
| [**01: How to Pick an Idea**](docs/01-HOW-TO-PICK-AN-IDEA.md) | The Three Filters for choosing a winning idea fast. |
| [**02: Team & Planning**](docs/02-TEAM-AND-PLANNING.md) | Roles, timeline, and scoping for a 24-48hr build. |
| [**03: Judging & Pitching**](docs/03-JUDGING-AND-PITCHING.md) | What judges actually score, and how to hack the rubric. |
| [**04: Demo Playbook**](docs/04-DEMO-PLAYBOOK.md) | The Critical Path demo scripts, video tips, and faking it. |
| [**05: Tech Stack Cheatsheet**](docs/05-TECH-STACK-CHEATSHEET.md) | Fast, reliable stacks by project type (Boring = Better). |
| [**06: Common Mistakes**](docs/06-COMMON-MISTAKES.md) | The traps that sink otherwise-good projects. |
| [**07: How to Stand Out**](docs/07-HOW-TO-STAND-OUT.md) | Story-driven demos, showing the learning curve, and the LinkedIn test. |

### Idea Bank (40+ Projects)
| Category | Link |
|---|---|
| **Master Index** | [**Browse the full mindmap**](docs/ideas/00-IDEA-INDEX.md) |
| **Memory Agents** | [Sales](docs/ideas/09-memory-agents-sales.md) / [Marketing](docs/ideas/10-memory-agents-marketing.md) / [Engineering](docs/ideas/11-memory-agents-engineering.md) / [Ops](docs/ideas/12-memory-agents-operations.md) / [Product](docs/ideas/13-memory-agents-product.md) |
| **AI & Agents** | [Browse ideas](docs/ideas/02-ai-and-agents.md) |
| **Productivity** | [Browse ideas](docs/ideas/01-productivity-tools.md) |
| **Fintech** | [General](docs/ideas/03-fintech.md) / [AI Finance Projects](docs/ideas/14-ai-finance-projects.md) |
| **Health & Wellness** | [Browse ideas](docs/ideas/04-health-and-wellness.md) |
| **Climate & Impact** | [Browse ideas](docs/ideas/05-sustainability-and-climate.md) |
| **Education** | [Browse ideas](docs/ideas/06-education.md) |
| **Social Good** | [Browse ideas](docs/ideas/07-social-good-and-accessibility.md) |
| **Developer Tools** | [Browse ideas](docs/ideas/08-developer-tools.md) |

### Community
| Resource | Link |
|---|---|
| **Submit an Idea** | [Contributing Guide](CONTRIBUTING.md) |
| **Community Rules** | [Code of Conduct](CODE_OF_CONDUCT.md) |

</details>

---

## Quick Start Scenarios

**Scenario 1: You have 2 hours until kickoff and no idea what to build.**
Read [`01-HOW-TO-PICK-AN-IDEA.md`](docs/01-HOW-TO-PICK-AN-IDEA.md) for the framework, then head straight to the [Idea Index](docs/ideas/00-IDEA-INDEX.md) and steal something.

**Scenario 2: You have an idea, but you don't know who should do what.**
Read [`02-TEAM-AND-PLANNING.md`](docs/02-TEAM-AND-PLANNING.md) and assign the "Demo Driver" role immediately. 

**Scenario 3: You are stuck in "Integration Hell" with 6 hours left.**
Drop everything and read [`06-COMMON-MISTAKES.md`](docs/06-COMMON-MISTAKES.md). Cut scope, hardcode the backend if you have to, and save the demo.

**Scenario 4: Your project actually works and you want to win.**
Spend your last 3 hours exclusively on [`03-JUDGING-AND-PITCHING.md`](docs/03-JUDGING-AND-PITCHING.md) and [`04-DEMO-PLAYBOOK.md`](docs/04-DEMO-PLAYBOOK.md). The best code doesn't win; the best 3-minute pitch wins.

---

## Contributing

We want your winning ideas! If you built something at a hackathon that blew the judges away, add it to our Idea Index. 
Check out our [Contributing Guide](CONTRIBUTING.md) to get started.

---

## The One-Sentence Version

> Pick a real problem, scope it down until you can actually finish it, and spend your last few hours on the demo : not new features.

<div align="center">
 <b>If this guide saved your weekend, drop a star on the repo!</b>
</div>

---

## License

MIT © [yashkoaprde](https://github.com/yashkoaprde)
