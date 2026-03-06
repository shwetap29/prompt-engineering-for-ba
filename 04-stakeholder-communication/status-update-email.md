# 📧 Status Update Email

**Level:** Beginner–Intermediate  
**Category:** Stakeholder Communication  
**Time Saved:** 15–20 min per update

---

## What This Is

A prompt that writes a clear, professional weekly project status email — with RAG status, progress highlights, upcoming milestones, and a specific call to action if a blocker exists.

---

## When to Use It

- Weekly or bi-weekly project status communications to sponsors or stakeholders
- When a milestone is hit, missed, or at risk
- When you need to flag a blocker to leadership without causing unnecessary alarm

---

## The Prompt

```
You are a Business Analyst writing a weekly project status update email 
to a non-technical business stakeholder or project sponsor.

Write a concise, professional email (under 200 words) that includes:
- Subject line
- RAG Status: 🟢 Green / 🟡 Amber / 🔴 Red — with one sentence explaining why
- 3 key accomplishments this week (bullet points, each under 15 words)
- 2–3 upcoming milestones with target dates
- One specific blocker or decision needed from the stakeholder (if any)
- A clear call to action if you need something from them

Project context: [2–3 sentences describing the project]
This week's progress: [paste your bullet notes — as rough as you like]
Blockers or decisions needed: [describe, or write "none this week"]
RAG Status to use: [Green / Amber / Red]
Tone: professional but warm — not stiff, not overly casual
```

---

## Filled Example

**Your input:**
```
Project: CRM reporting dashboard for the Sales team.
Progress: finished wireframes, got sign-off on KPI list, dev started 
on the revenue widget.
Blocker: still waiting on database access credentials from IT for 10 days.
RAG: Amber
```

**AI Output:**

---

**Subject:** CRM Dashboard — Weekly Status Update | 🟡 Amber

Hi [Name],

Here's this week's update on the CRM Reporting Dashboard.

**Status: 🟡 Amber** — On track overall, but an outstanding IT access request is at risk of impacting the development timeline if not resolved by Wednesday.

**This Week:**
- Wireframes completed and signed off by stakeholders ✅
- Final KPI list confirmed — 12 metrics approved for Phase 1 ✅
- Development started on the Revenue by Region widget ✅

**Coming Up:**
- UAT kick-off: March 15
- Go-live target: March 28

**Action Needed:**
We've been waiting 10 days for database access credentials from IT. Could you help escalate this with the IT team? We need access by Wednesday to protect the development timeline.

Happy to jump on a quick call if helpful.

[Your name]

---

## Tips

- 🟡 Amber is your best friend — use it proactively when a risk exists, before it becomes Red
- Keep "Action Needed" to one specific ask — multiple requests in one email get ignored
- If there's no blocker, replace the action section with a positive forward-looking note
- Reuse this structure every week — consistency builds stakeholder trust over time
