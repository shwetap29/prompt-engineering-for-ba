# 🔄 Iterative Refinement

**Level:** Advanced  
**Category:** Advanced Techniques  
**Builds on:** All previous prompts

---

## What This Is

Iterative refinement is the technique of improving an AI output through a series of follow-up instructions — rather than trying to write one perfect prompt, or starting over when the first response isn't quite right.

Think of it like editing a draft with a colleague. You don't throw away draft 1 — you give specific feedback and build on it.

---

## Why This Changes Everything

Most people use AI like this:
1. Write a prompt
2. Get output
3. Copy and edit it manually

Power users use AI like this:
1. Write a first prompt (doesn't have to be perfect)
2. Get output
3. Give specific refinement instructions
4. Get improved output
5. Repeat until it's right

The second approach is faster, produces better results, and teaches you what works.

---

## The Refinement Instruction Library

Copy any of these into a follow-up message after your first AI response:

### Length & Conciseness
```
Make this more concise — cut it to under 150 words without losing the key points.
Remove any repeated ideas and tighten every sentence.
Shorten this to a 3-sentence version I can use as a slide headline.
```

### Tone & Audience
```
Rewrite this for a non-technical business audience — remove all jargon.
Make the tone warmer and more conversational — it's too formal right now.
Rewrite this as if you're writing for a C-suite audience, not a project team.
```

### Structure & Format
```
Restructure this as a table instead of bullet points.
Add a summary section at the top with the 3 most important points.
Break this into clearly labelled sections with bold headers.
Convert this into a numbered step-by-step list.
```

### Adding Depth
```
Add a "risks and mitigation" section at the end.
Add 2 open questions that still need stakeholder input.
Include a recommendation for each finding.
Now add a second perspective — what would a sceptical stakeholder push back on?
```

### Rewriting Sections
```
The second paragraph is too vague — rewrite it with more specifics.
The opening sentence is weak — rewrite it to lead with the most important point.
The action items table is missing due dates — add a column and infer reasonable timelines.
```

---

## Real BA Example — Refining a BRD Section

**Prompt 1 (first draft):**
```
You are a senior BA. Write a BRD section for a new expense approval 
workflow based on these notes: [paste notes]
```

**AI Response:** Produces a decent first draft but the scope section is vague and the requirements are too high-level.

---

**Prompt 2 (refine scope):**
```
The scope section is too vague. Rewrite it to be more specific — 
list 4–5 concrete in-scope items and 3 explicit out-of-scope exclusions 
based on the original notes.
```

---

**Prompt 3 (refine requirements):**
```
The functional requirements are too high-level. Rewrite them so each 
one starts with "The system shall..." and is specific enough for a 
developer to build from without asking a follow-up question.
```

---

**Prompt 4 (final polish):**
```
Now review the full document for consistency — make sure the scope, 
requirements, and assumptions all align with each other. 
Flag any contradictions.
```

Four prompts. One high-quality BRD section. Each step took 30 seconds.

---

## The Golden Rule of Iteration

> **Never start over. Always build forward.**

If the output isn't right, describe *specifically what's wrong* and ask AI to fix that part. Starting over from scratch wastes everything the AI has already learned about your context in this conversation.

---

## Tracking What Works

When an iterative sequence produces a great output, save the full prompt chain — not just the final result. Next time you do a similar task, you have a repeatable process.

Example of what to save:
```
Task: BRD section from stakeholder notes
Prompt 1: [initial prompt]
Prompt 2: "Tighten the scope section..."
Prompt 3: "Rewrite requirements as 'The system shall...' statements"
Prompt 4: "Check for consistency across sections"
Result: Production-ready BRD in ~5 minutes
```

---

## Tips

- Start with a decent-but-imperfect prompt — don't spend 15 minutes on prompt 1
- Give feedback the way you'd brief a smart colleague: specific, constructive, clear
- Three to five iterations is usually enough to get a polished, professional output
- Keep your conversation open — don't close the chat. AI remembers everything in the current session
