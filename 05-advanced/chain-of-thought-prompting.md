# 🔗 Chain-of-Thought Prompting

**Level:** Advanced  
**Category:** Advanced Techniques  
**Builds on:** The 4-Part Formula, Role Prompting

---

## What This Is

Chain-of-thought (CoT) prompting asks AI to **think through a problem step-by-step before giving you the answer** — rather than jumping straight to a conclusion.

This dramatically improves output quality for analytical tasks, complex decisions, and multi-part problems.

---

## Why It Works

When you ask AI for a direct answer to a complex question, it sometimes skips steps, misses nuance, or gives you a confident but shallow response.

When you tell it to *show its reasoning first*, it catches its own errors, considers more angles, and produces a more reliable answer.

Think of it like asking a smart colleague to "talk me through your thinking" rather than just "give me the answer."

---

## The Basic Pattern

Add one of these phrases to any prompt:

```
"Think through this step by step before giving your final answer."
"Walk me through your reasoning before concluding."
"Before answering, list the key considerations you're weighing."
"First analyse the problem, then provide your recommendation."
```

---

## BA Example — Prioritising Requirements

**Without Chain-of-Thought (shallow output):**
```
Which of these requirements should we build first?
[list of requirements]
```
AI gives you a ranked list with thin justification.

---

**With Chain-of-Thought (deeper output):**
```
You are a senior Business Analyst helping a product team prioritise 
a backlog for the next sprint.

Before giving your final prioritisation, think through:
1. Which requirements are blocking other requirements (dependencies)?
2. Which have the highest business value based on the context given?
3. Which carry the most delivery risk if delayed?
4. Which are quick wins vs. high effort?

Then give your final prioritised list with a one-line rationale for 
each item.

Requirements:
[PASTE YOUR REQUIREMENTS LIST HERE]

Business context: [describe the product, users, and current sprint goal]
```

---

## DA Example — Diagnosing a KPI Drop

**Without Chain-of-Thought:**
```
Why did revenue drop 15% this month?
[paste data]
```
AI gives generic reasons.

---

**With Chain-of-Thought:**
```
You are a Data Analyst diagnosing a revenue decline for a business 
stakeholder.

Before giving your conclusion, work through each of these diagnostic 
questions using the data provided:

1. Is the drop concentrated in one segment (region, product, customer type) 
   or spread across all segments?
2. Did the number of transactions drop, or did the average transaction 
   value drop, or both?
3. Is this a one-time anomaly or part of a trend visible in prior periods?
4. What external factors (seasonality, promotions, market events) could 
   explain this?

After working through each question, give your top 2–3 most likely 
root causes with supporting evidence from the data.

Data:
[PASTE YOUR DATA HERE]
```

---

## When to Use Chain-of-Thought

| Use it when... | Skip it when... |
|---|---|
| The problem has multiple variables | You just need a quick draft or simple output |
| You want AI to catch its own errors | The task is straightforward and well-defined |
| You need to justify a recommendation | Speed is more important than depth |
| The output will be presented to senior stakeholders | You're iterating on something and will review anyway |

---

## Tips

- The longer and more analytical the task, the more CoT helps
- You can also ask AI to show its reasoning *after* the answer: *"Now explain your reasoning for each recommendation"*
- CoT is particularly powerful combined with role prompting — the right persona + step-by-step reasoning = expert-level output
- See `role-persona-prompting.md` for how to combine these two techniques
