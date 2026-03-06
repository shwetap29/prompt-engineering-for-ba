# 🔍 Anomaly Explainer

**Level:** Intermediate  
**Category:** Data Insights  
**Time Saved:** 20–30 min per explanation

---

## What This Is

A prompt that helps you write a clear, calm, professional explanation when a data anomaly needs to be communicated to a non-technical stakeholder — without alarming them or being dismissive.

---

## When to Use It

- A KPI has moved significantly and stakeholders will ask why
- A report shows a number that looks wrong — and you need to communicate it before being asked
- You've identified a data quality issue and need to explain it clearly

---

## The Prompt

```
You are a Business Analyst explaining a data anomaly to a non-technical 
business stakeholder. They are not a data person — they need plain language 
and a clear path forward.

Write a short, professional explanation that includes:

1. What happened — describe the anomaly in plain language (no jargon)
2. Why it might have occurred — list 2–3 possible causes
3. What has been investigated so far — and what has been ruled out
4. What the next step is — one specific, clear action

Anomaly: [describe what you found — metric name, the unexpected value, timeframe]
Data source: [where does this data come from?]
Business context: [why does this metric matter?]
What you've checked so far: [or write "investigation just started"]
Tone: calm, factual, and solution-focused — not alarming
Format: short paragraphs with a bold label on each section
```

---

## Filled Example

**Your input:**
```
Anomaly: Website conversion rate dropped from 4.2% to 1.8% overnight on 
March 5th — a 57% drop.
Data source: Google Analytics dashboard
Business context: conversion rate feeds directly into the weekly revenue forecast
What you've checked: tracking code — no changes. Active campaigns — none paused.
```

**AI Output:**

---

**What happened**  
Our website conversion rate fell from 4.2% to 1.8% on March 5th — roughly half the normal rate. This means that for every 100 visitors to the site that day, only 1–2 completed a purchase, compared to around 4 on a typical day.

**Possible causes**  
1. A technical issue with the checkout process — a broken button, page error, or payment failure could silently block completions without showing an obvious error to users  
2. A tracking gap — if the conversion event tag stopped firing correctly, completions may have happened but not been recorded  
3. A traffic quality shift — if the traffic source changed significantly (e.g., a paid campaign paused), the remaining audience may naturally convert at a lower rate

**What's been checked**  
The analytics tracking code has been reviewed — no changes were made on or before March 5th. No active campaigns were paused. The anomaly appears isolated to a single day.

**Next step**  
The web development team has been asked to review the checkout flow and error logs for March 5th. We will confirm root cause and provide an update by [date].

---

## Tips

- Always lead with the facts, not the alarm — calm communicators build more trust
- If you genuinely don't know the cause, say "possible reasons" not "the reason is..."
- Pair this with a screenshot of the anomaly when sending to stakeholders — it adds clarity
- Close the loop: once resolved, send a one-line follow-up: *"Root cause confirmed — [brief summary]. Issue resolved as of [date]."*
