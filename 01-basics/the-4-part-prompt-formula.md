# 🧩 The 4-Part Prompt Formula

**Level:** Beginner  
**Time to read:** 7 minutes

---

## The Formula Every Prompt in This Repo Uses

```
[ROLE] + [TASK] + [CONTEXT] + [FORMAT]
```

You don't need to use all four every time — but the more you include, the better the output.

---

## Breaking It Down

### Part 1 — ROLE
Tell the AI who to be before you give it any task.

This single change improves output quality more than anything else.

```
"You are a senior Business Analyst..."
"You are a data analyst presenting to a non-technical audience..."
"You are a QA engineer reviewing acceptance criteria..."
```

**Why it works:** AI adjusts its vocabulary, assumptions, and depth based on the role. A "senior BA" will write differently than just "an assistant."

---

### Part 2 — TASK
Tell the AI exactly what you want it to produce.

Be specific. Vague tasks = vague output.

```
❌  "Write something about requirements"
✅  "Write a Business Requirements Document section with objectives, scope, and functional requirements"

❌  "Summarise this data"
✅  "Write a 4-sentence executive summary leading with the most important finding"
```

---

### Part 3 — CONTEXT
Give the AI the raw material it needs. This is where you paste your actual work.

```
"Based on the following stakeholder notes: [PASTE HERE]"
"Using this KPI data: [PASTE TABLE HERE]"
"Here is the user story to review: [PASTE HERE]"
```

**Rule:** The more specific and real your context, the more useful and tailored the output. Never leave this section vague.

---

### Part 4 — FORMAT
Tell the AI how to structure its response.

```
"Use headers and a numbered list"
"Write in a table with columns: Requirement | Priority | Owner"
"Keep it under 200 words"
"Use Gherkin format: Given / When / Then"
"Write in bullet points, each one 1–2 sentences"
```

---

## The Full Formula in Action

Here's how all 4 parts come together for a real BA task:

```
[ROLE]
You are a senior Business Analyst with experience in Agile delivery.

[TASK]
Write 3 user stories with acceptance criteria for the following feature request.
Use the format: "As a [user], I want [action] so that [benefit]."
For each story, write 3 acceptance criteria in Gherkin format (Given / When / Then).

[CONTEXT]
Feature request from the product team:
"Managers need to be able to approve or reject employee timesheets 
directly from their dashboard, and employees should be notified of 
the decision by email."

[FORMAT]
Structure the output as:
- User Story (bold)
- Acceptance Criteria (bulleted, Gherkin format)
Separate each story with a horizontal line.
```

---

## Cheat Sheet — Swap These In

**ROLE options for BAs and DAs:**
- `You are a senior Business Analyst with 10 years of enterprise experience...`
- `You are a Data Analyst presenting insights to a non-technical executive...`
- `You are a QA-focused BA reviewing requirements for testability...`
- `You are a project coordinator writing stakeholder communications...`

**FORMAT options:**
- `Use a table with columns: [column names]`
- `Write in bullet points, max 10 words per bullet`
- `Use numbered steps`
- `Keep the entire response under 150 words`
- `Use headers for each section`

---

## Quick Reference Card

| Part | Question It Answers | If You Skip It... |
|---|---|---|
| Role | Who is writing this? | Output is generic, not expert-level |
| Task | What should be produced? | AI guesses and often guesses wrong |
| Context | What material to work from? | AI invents details that aren't true |
| Format | How should it look? | Output structure is unpredictable |

---

## Next Step
→ Try `your-first-5-prompts.md` — five ready-to-use prompts for your first week.
