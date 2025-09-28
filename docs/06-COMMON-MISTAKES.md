---
title: Common Mistakes
author: yashkoaprde
part_of: Yash Hackathon Guide
---

# Common Mistakes

[← Back to README](../README.md) · [← Tech Stack Cheatsheet](05-TECH-STACK-CHEATSHEET.md)

Things that quietly sink otherwise-good hackathon projects, roughly in order of how often they happen. Avoid these traps.

---

## 1. Planning Mistakes

- **Picking an idea too big to finish.** The single most common failure. If your app needs 5 different screens to make sense, it's too big. See [How to Pick an Idea](01-HOW-TO-PICK-AN-IDEA.md).
- **No clear owner per task.** "We'll figure it out together" leads to duplicated work and gaps. Assign explicit ownership even in a 2-person team.
- **Skipping the halfway checkpoint.** Teams that don't stop to honestly assess progress at the midpoint tend to discover they're behind only when it's too late to adjust.
- **Building breadth before depth.** Five half-working features score worse than one fully-working core loop. Always finish the core loop first.

---

## 2. Building Mistakes

- **No error handling anywhere.** A demo that crashes on an unexpected input in front of judges is brutal. Wrap external calls (APIs, file uploads, user input) in try/catch blocks.
- **Hardcoding the happy path only.** If your only tested scenario is the exact one in your demo script, any deviation during Q&A will break it.
- **Ignoring the loading state.** API calls that take 3+ seconds with no visual feedback look broken. Add a spinner. 
- **Not testing on the actual demo network.** Hackathon Wi-Fi is notoriously bad. Test your deployed app on the venue network before you get on stage.

---

## 3. Design & Data Mistakes

- **Obviously fake demo data.** "Test123", "asdf@asdf.com," everything dated today. Judges read sloppy data as a signal the team didn't care. Use an LLM to generate 20 rows of realistic fake data.
- **Default, unstyled UI.** Even 30 minutes of basic spacing, color, and typography reads as "finished" instead of "prototype."
- **Cluttered screens for the demo.** Hide anything not relevant to the story you're telling. Delete the debug panels and unused nav items before presenting.

---

## 4. Pitch Mistakes

- **Leading with tech stack instead of the problem.** Judges connect with the "why" before the "how." 
- **No specific numbers or scenario.** Vague claims ("this saves time") are forgettable; specific ones ("cuts a 20-minute task to 90 seconds") stick.
- **Apologizing for unfinished parts.** Present what works confidently. Frame gaps as an intentional future roadmap, not excuses.
- **Going over time.** Judges will cut you off mid-sentence. A shorter, complete pitch is much better than a long one that gets interrupted.
- **Not rehearsing out loud.** Reading a script silently and speaking it out loud for the first time in front of judges are very different experiences. Rehearse for real.

---

## The "Oh Crap" Emergency Checklist

If you have 4 hours left and nothing works, do this:

- [ ] **Stop building new things.** Put pencils down.
- [ ] **Identify the core demo.** What is the absolute minimum you need to show?
- [ ] **Hardcode everything else.** If the database connection broke, delete the connection and hardcode a JSON array in the frontend. 
- [ ] **Fix the CSS.** A hardcoded app that looks beautiful will score higher than a fully functional backend with an unstyled HTML form.
- [ ] **Practice the pitch.** 

---
Maintained by [@yashkoaprde](https://github.com/yashkoaprde)

[← Back to README](../README.md)
