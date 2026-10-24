# Finding & Selecting Hackathons

> "Not every hackathon is worth your weekend. Choose events where you maximize learning, build relationships, and tackle meaningful problems."

Finding the right hackathon is a strategic decision. Applying randomly without evaluating the tracks, judging composition, or tech requirements often leads to burnout. Here is how to systematically discover, filter, and qualify hackathons.

---

## 1. Top Hackathon Discovery Platforms

Keep bookmarks for these platforms to catch application windows early:

```mermaid
flowchart TD
    Hub["Hackathon Discovery Ecosystem"]
    Hub --> D["Devfolio<br/>(ETHIndia, InOut, Top Collegiate)"]
    Hub --> U["Unstop<br/>(SIH, Tata, Flipkart, National)"]
    Hub --> DP["Devpost<br/>(Global Cloud & AI Challenges)"]
    Hub --> M["MLH<br/>(Major League Hacking Student Circuit)"]
    Hub --> C["Internal Campus Sprints<br/>(e.g., 31 October 2026 Mini Hackathon)"]

    style Hub fill:#fff2a6,stroke:#fbc02d,stroke-width:2px
    style C fill:#e8f5e9,stroke:#388e3c,stroke-width:2px
```

| Platform | Primary Focus | Best For | Typical Format |
|---|---|---|---|
| **[Devfolio](https://devfolio.co)** | High-quality developer hackathons (ETHIndia, HackOut) | Web3, AI, full-stack, collegiate circuits | In-person & Online |
| **[Unstop](https://unstop.com)** | Indian university competitions & national challenges | College students, hiring challenges, SIH | Hybrid / Multi-stage |
| **[Devpost](https://devpost.com)** | Global software hackathons & sponsor challenges | Cloud APIs, LLM hackathons, global submissions | Primarily Online |
| **[Major League Hacking (MLH)](https://mlh.io)** | Student hackathon league across North America, Europe, Asia | Beginner tracks, collegiate workshops | In-person & Online |
| **Campus Sprints** | Beginner-friendly local collegiate sprints (e.g. 31 Oct 2026) | First-year developers, rapid MVPs | In-Person Labs |

---

## 2. Event Qualification Decision Tree

Before committing your weekend, run the prospective event through this decision flowchart:

```mermaid
flowchart TD
    Q1{"Is the theme open or strictly restricted?"}
    Q1 -- "Overly restricted to legacy stack" --> Skip["SKIP / LOW PRIORITY<br/>(Restricts creativity & modern stacks)"]
    Q1 -- "Open or aligned with team stack" --> Q2{"Are there experienced mentors available?"}
    Q2 -- "No mentors / purely asynchronous" --> Q3{"Is there a specific sponsor API bounty?"}
    Q2 -- "Yes, hands-on mentorship" --> Green["APPLY IMMEDIATELY ✅<br/>(High learning ROI)"]
    Q3 -- "Yes, clear side prizes" --> Green
    Q3 -- "No, vague judging & no support" --> Skip
```

### The 5-Point Evaluation Filter:
1. **Theme Alignment & Technical Freedom:** Does the event permit modern tooling (Next.js, FastAPI, Supabase, [iNSIGHTS AI](https://insights-ai.info))?
2. **Team Sizing & Eligibility:** Does your squad match the eligibility criteria (e.g., first-year undergraduate focus)?
3. **Sponsor Tracks & Side Bounties:** Are there targeted sponsor bounties (e.g., "Best AI Integration")? Targeting niche bounties is a proven route to winning prizes even if you miss the overall podium.
4. **Logistics & Health:** For offline events, are electrical surge protectors, Wi-Fi, food, and mentor tables arranged?
5. **Mentorship ROI:** Will you receive feedback from seasoned engineers that improves your craft?

---

## 3. Assembling a High-Performing Squad

Avoid forming a team of four frontend developers who dislike databases, or four backend developers who cannot style a button.

```mermaid
flowchart TD
    subgraph TheBalancedSquad [The 4-Member Winning Squad Archetype]
        B["1. The Builder (Frontend / UI)<br/>Next.js • Tailwind • shadcn/ui<br/>Zero blank states & smooth interactions"]
        A["2. The Architect (Backend / AI)<br/>FastAPI • Python • Schemas<br/>API contracts & database pipelines"]
        S["3. The Storyteller (Product / Pitch)<br/>Problem validation • iNSIGHTS AI research<br/>7-slide deck & stage presentation"]
        I["4. The Integrator (QA & DevOps)<br/>Edge case testing • Offline backup video<br/>README setup & deployment smoke test"]
    end
```

---

## 4. Application Crafting: Getting Accepted

Competitive hackathons require an application review. Here is what selection committees look for:

- **Past Proof of Work:** Include links to active GitHub profiles, deployed live projects, or concise portfolio write-ups.
- **Genuine Motivation:** Avoid boilerplate responses ("I want to learn technology"). Instead, state: *"Our team wants to explore how local language document intelligence can assist small retail businesses in Karnataka."*
- **Diversity of Thought:** Highlight distinct perspectives or domain interest (e.g., combining agriculture domain knowledge with software engineering).

---

## 5. Next Steps

- Move into problem discovery: **[Research & Ideation](research-and-ideation.md)**
- Check the official operating manual: **[Mini Hackathon Overview](../mini-hackathon/event-overview.md)**
