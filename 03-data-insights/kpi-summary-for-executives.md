# 📊 KPI Summary for Executives

**Level:** Intermediate  
**Category:** Data Insights  
**Time Saved:** 30–45 min per summary

---

## What This Is

A prompt that turns a set of KPI values into a clear, confident, plain-language executive narrative — the kind a senior leader can read in 30 seconds and immediately act on.

---

## When to Use It

- Writing the "insights" or "commentary" section of a dashboard or report
- Preparing talking points before a business review meeting
- Adding a narrative paragraph to a monthly reporting pack or Power BI export

---

## The Prompt

```
You are a Business Analyst writing an executive performance summary for 
a senior leader who wants plain language, not data tables.

Using the KPI data below, write a summary of 4–6 sentences that:

1. Opens with a one-sentence headline — the single most important takeaway
2. Highlights what is performing well (with numbers)
3. Highlights what is underperforming or at risk (with numbers)
4. Identifies the most likely driver of the biggest variance
5. Closes with one clear, specific recommendation for next steps

KPI Data:
[PASTE YOUR KPIS, ACTUALS, AND TARGETS HERE]

Reporting period: [e.g., February 2026]
What decision does this data need to inform: [one sentence]
Audience: [e.g., C-suite / Department Head / Client]
Tone: confident, direct, data-backed — no hedging phrases like "it seems" or "possibly"
```

---

## Filled Example

**Your input:**
```
Period: February 2026
Revenue: $1.85M actual vs $2.0M target (-7.5%)
New Customers: 142 actual vs 120 target (+18%)
Retention Rate: 91% actual vs 90% target (+1pp)
Average Order Value: $310 actual vs $350 target (-11%)
Support Resolution Time: 4.2 hrs actual vs <6 hrs target (✅)

Decision to inform: Q1 budget reallocation
Audience: VP of Sales
```

**AI Output:**

> February delivered strong customer acquisition and retention but fell $150K short of revenue target, driven entirely by compression in average order value.
>
> Acquisition exceeded target by 18% (142 new customers vs. goal of 120), and retention held above target at 91% — both indicating healthy customer engagement. Support resolution time also remained well inside the 6-hour benchmark.
>
> The primary gap is average order value: at $310 against a $350 target, customers are transacting more frequently but spending less per order. This 11% shortfall accounts for the full revenue miss and likely reflects either the current promotional discount depth or a shift in product mix toward lower-price items.
>
> For Q1 budget, recommend reviewing promotional discount thresholds and introducing upsell prompts at checkout — both are low-cost levers to recover AOV without impacting the strong acquisition momentum.

---

## Tips

- If your data is in Excel or Power BI, copy the table directly into the prompt — AI reads it cleanly
- Always check that every number AI includes matches your source data exactly
- Follow up with: *"Now write a 2-sentence version for a slide headline"*
- Follow up with: *"Now write a version for a client audience, not internal"*
