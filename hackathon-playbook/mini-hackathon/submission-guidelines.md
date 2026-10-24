# Mini Hackathon: Submission Guidelines

> "If it isn't documented and submitted before the portal timer reaches 00:00, it doesn't exist."

Every team must complete their project submission through the designated portal before the official code freeze deadline. Review this guide to ensure your submission meets all verification checks.

---

## 1. Mandatory Deliverables

Each team submission must include five components:

```
┌─────────────────────────────────────────────────────────────┐
│ 1. Public GitHub Repository Link with Active Commit History │
├─────────────────────────────────────────────────────────────┤
│ 2. Well-Structured README.md with Setup Instructions        │
├─────────────────────────────────────────────────────────────┤
│ 3. Working Live URL OR Local Execution Instructions         │
├─────────────────────────────────────────────────────────────┤
│ 4. Pitch Deck (PDF or Google Slides View Link)              │
├─────────────────────────────────────────────────────────────┤
│ 5. 60–90 Second Screen-Recorded Backup Demo Video           │
└─────────────────────────────────────────────────────────────┘
```

### Deliverable Specifications:

1. **GitHub Repository:**
   - Must be set to **Public** during evaluation.
   - Must contain atomic commits reflecting team progress throughout the sprint.
   - Must include an open-source license (e.g., MIT).
2. **README.md:**
   - Must follow the [Project README Template](../templates/project-readme.md).
   - Must list the problem statement, core features, architecture diagram, tech stack, and step-by-step local setup steps.
3. **Live Deployment / Prototype:**
   - Deployed link (Vercel, Render, Netlify, Streamlit, or Expo Snack).
   - If running locally (e.g., hardware/local model), code must run with clear commands (`npm run dev` or `python main.py`).
4. **Pitch Deck:**
   - Exported as a PDF or accessible view-only link (ensure permissions are set to *"Anyone with the link can view"*).
   - Maximum 7 slides following the [Pitch Deck Template](../templates/pitch-deck.md).
5. **Backup Demo Video:**
   - Hosted on YouTube (Unlisted), Loom, or Google Drive (public access).
   - Maximum length: 90 seconds demonstrating the core user flow.

---

## 2. Pre-Submission Self-Audit Checklist

Before pressing the submit button, run this 5-minute sanity check:

- [ ] **Incognito Link Check:** Open your GitHub repo and live URL in an Incognito / Private browser tab. Does it load without login walls?
- [ ] **Permission Verification:** Is your Google Slides or Drive video set to *"Anyone on the internet with the link can view"*?
- [ ] **No Secrets Exposed:** Ensure `.env` is listed in your `.gitignore`. Check that no OpenAI, Anthropic, or database passwords were committed to GitHub history.
- [ ] **Dependencies Documented:** Is `package.json` or `requirements.txt` up to date with all installed libraries?
- [ ] **Team Members Listed:** Are all registered members and their contributions noted in the README?

---

## 3. Late Submissions Policy

- The submission portal locks automatically at the announced deadline.
- Submissions timestamped after the cutoff will receive a **10-point late penalty per 5 minutes of delay** up to 15 minutes, after which the submission will not be considered for podium awards.
- Technical emergencies must be flagged to an organizer *before* the deadline passes.

---

## 4. Next Steps

- Prepare the organizer operational checklist: **[Organizer Checklist](organizer-checklist.md)**
- Review the markdown layout: **[Project README Template](../templates/project-readme.md)**
