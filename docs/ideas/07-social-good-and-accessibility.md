---
title: Social Good & Accessibility
author: yashkoaprde
part_of: Yash Hackathon Guide
---

# Social Good & Accessibility

[← Back to Idea Index](00-IDEA-INDEX.md) · [← Education](06-education.md)

| Idea | Problem | MVP Demo | Advanced Scope | Anti-pattern |
|---|---|---|---|---|
| **Plain-Language Form/Document Translator** | Government forms, legal notices, and benefits applications are often written at a reading level that excludes many of the people who need them most : a real barrier to accessing services people are entitled to. | Upload/paste a dense document → rewrite in plain language at a target reading level → preserve critical details (deadlines, required actions) prominently, never silently drop them. | | Cut: multi-language translation (start with plain-language English, add languages if time allows). Add if time allows: highlighting exactly which original sentence each simplified sentence came from, for trust/verification. |
| **Screen-Reader-First Navigation Aid for Complex Websites** | Many essential websites (benefits portals, healthcare systems) are poorly optimized for screen readers, making basic tasks exhausting or impossible for blind and low-vision users. | Browser extension/overlay that restructures a page's content into a clean, logical screen-reader-friendly flow → test with an actual screen reader during development, not just visually. | | Cut: working on every possible website (pick 1-2 realistic target sites for the demo). Add if time allows: voice-command navigation on top of the restructured flow. |
| **Volunteer-to-Need Matcher for Local Nonprofits** | Small nonprofits often can't efficiently match specific volunteer skills (translation, accounting, tech support) to specific one-off needs : most volunteer platforms are built for large recurring shifts, not niche one-time asks. | Nonprofits post specific, skill-tagged needs → volunteers list their specific skills/availability → match on skill overlap, not just general "I want to volunteer" sign-ups. | | Cut: scheduling/calendar sync. Add if time allows: a simple reputation system based on completed matches. |
| **Sign Language Practice Companion** | Learning sign language is hard without a fluent practice partner, and most learning apps focus on vocabulary flashcards rather than real conversational practice. | Use a pretrained sign-recognition model (many open-source options exist) → give the user a phrase to sign → provide real-time feedback on accuracy, not just a video reference. | | Cut: full conversational fluency assessment. Add if time allows: a small curated phrase-set progression (beginner → intermediate). |
| **Disaster/Emergency Resource Locator for Non-English Speakers** | During emergencies (weather events, evacuations), critical resource information (shelters, aid stations) is often only published in the dominant local language, excluding non-native speakers when it matters most. | Aggregate/mock a set of emergency resource listings → present with location, hours, and required documents → auto-translate into multiple languages, prioritizing clarity over literal translation. | | Cut: live official data feeds (use realistic mock data for the demo). Add if time allows: offline-accessible mode, since emergencies often disrupt connectivity. |

---
Maintained by [@yashkoaprde](https://github.com/yashkoaprde)
