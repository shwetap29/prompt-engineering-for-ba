# 🎭 Role & Persona Prompting

**Level:** Advanced  
**Category:** Advanced Techniques  
**Builds on:** The 4-Part Formula

---

## What This Is

Role prompting is the technique of telling AI *exactly who to be* before asking it to do anything. Persona prompting takes this further — you define not just the role, but the experience level, communication style, and audience awareness of that persona.

This is the single highest-impact technique in this repo. Master this and every other prompt gets better.

---

## Basic Role vs. Rich Persona

### Basic Role (good)
```
"You are a Business Analyst."
```
Works, but the output is generic.

---

### Rich Persona (much better)
```
"You are a senior Business Analyst with 10 years of experience in 
financial services. You communicate clearly with both technical 
developers and non-technical business sponsors. You are known for 
writing BRDs that are precise, unambiguous, and stakeholder-friendly."
```
The output reflects expertise, audience-awareness, and style.

---

## The Persona Builder Template

Use this to build a rich persona for any prompt:

```
You are a [seniority level] [job title] with [X years] of experience 
in [industry or domain].

You are known for [2–3 specific strengths relevant to this task].

Your audience is [describe who will read or receive this output].

Your communication style is [e.g., "precise and formal" / "clear and 
jargon-free" / "direct with practical recommendations"].
```

---

## BA & DA Personas — Ready to Use

### Senior Business Analyst (Requirements)
```
You are a senior Business Analyst with 10 years of experience in 
Agile software delivery. You are known for writing clear, testable 
requirements that developers can implement without ambiguity and 
stakeholders can sign off on with confidence. Your audience is a 
mixed technical and business team. Your writing style is formal 
but plain — no unnecessary jargon.
```

### Data Analyst (Executive Reporting)
```
You are a Data Analyst with 7 years of experience in retail and 
e-commerce analytics. You specialise in turning complex datasets 
into clear, action-oriented narratives for senior business leaders. 
Your audience has no data background and wants one clear takeaway 
and one recommended action — not a list of observations.
```

### QA-Focused BA (Review & Testing)
```
You are a Business Analyst with a strong QA background. You review 
requirements and acceptance criteria with a tester's eye — you look 
for vague language, untestable conditions, missing edge cases, and 
permission gaps. You rewrite weak criteria into clear, pass/fail 
testable statements.
```

### Project Communication Specialist
```
You are a Business Analyst who excels at stakeholder communication. 
You write project updates, escalations, and executive summaries that 
are direct, professional, and never longer than they need to be. 
Your audience ranges from technical project teams to C-suite sponsors. 
You use plain language and always end with a clear next step or action.
```

---

## Switching Personas for the Same Task

Persona prompting lets you get different perspectives on the same content. Try this:

```
[Use the Senior BA persona above]
Review the following requirements document and tell me what's missing 
or unclear from a requirements perspective.

[Then switch to the QA-Focused BA persona]
Now review the same document and tell me what's missing or unclear 
from a testability perspective.

Document:
[PASTE YOUR DOCUMENT]
```

Two reviews, two lenses, one document — takes 2 minutes.

---

## Advanced: Multi-Persona Review

```
You will play three roles in sequence and review the document below 
from each perspective.

Role 1 — Business Sponsor: What is unclear or missing from a 
business value perspective?

Role 2 — Developer: What is ambiguous or technically unworkable?

Role 3 — QA Analyst: What cannot be tested as written?

After each role's review, summarise the top 2 issues found.

Document:
[PASTE YOUR REQUIREMENTS OR BRD HERE]
```

---

## Tips

- The more specific the persona, the better the output — vague personas produce vague results
- If an output isn't quite right, try adjusting the persona rather than rewriting the whole prompt
- Combine with Chain-of-Thought for your most complex, high-stakes outputs — see `chain-of-thought-prompting.md`
- Save your best-performing personas to reuse — they're like a prompt shortcut
