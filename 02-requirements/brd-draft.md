# 📄 BRD Section Draft

**Level:** Intermediate  
**Category:** Requirements  
**Time Saved:** 45–60 min per BRD section

---

## What This Is

A prompt that converts raw stakeholder meeting notes into a structured Business Requirements Document (BRD) section — formatted, professional, and ready for review.

---

## When to Use It

- Right after a discovery call or requirements workshop
- When you have rough notes and need a clean first draft fast
- Before circulating requirements for stakeholder sign-off

---

## The Prompt

```
You are a senior Business Analyst with experience writing formal Business 
Requirements Documents (BRDs) for enterprise software and reporting projects.

Based on the raw stakeholder notes below, write a professional BRD section 
that includes:

1. Business Objective
   One clear sentence: what is the business trying to achieve?

2. Scope
   - In-Scope: what this project/feature includes
   - Out-of-Scope: what is explicitly excluded (even if unstated — infer sensibly)

3. Functional Requirements
   Numbered list. Each requirement must start with: "The system shall..."

4. Assumptions
   Things being treated as true without formal confirmation

5. Open Questions
   Unresolved items that need stakeholder input before development begins

Stakeholder Notes:
[PASTE YOUR RAW NOTES HERE]

Audience: both a technical development team AND a non-technical business sponsor  
Tone: formal, precise, no jargon  
Format: use the 5 numbered sections above with bold headers
```

---

## Filled Example

**Your raw notes:**
```
The sales team wants a weekly report showing revenue by region. They want 
to filter by product category. Report goes out Mondays by 9am. Finance 
also wants margin % next to revenue. YoY comparison maybe later — not 
confirmed. US regions only for now.
```

**AI Output:**

---

**1. Business Objective**  
Enable the Sales and Finance teams to monitor weekly regional revenue performance and margin health, supporting faster commercial decision-making.

**2. Scope**  
In-Scope: Weekly revenue report segmented by US region; product category filter; margin % alongside revenue; automated Monday 9am delivery.  
Out-of-Scope: Year-over-Year comparison (deferred, Phase 2 candidate); non-US regions.

**3. Functional Requirements**  
1. The system shall generate a weekly revenue report segmented by US region.  
2. The system shall provide a product category filter on the report view.  
3. The system shall display margin percentage alongside revenue figures for each region.  
4. The system shall automatically distribute the report each Monday by 9:00 AM.

**4. Assumptions**  
- Revenue data is available and accurate in the source system by end of Sunday  
- "US regions" refers to the existing regional segmentation in the current data model  
- Margin % calculation uses gross margin (revenue minus COGS)

**5. Open Questions**  
- Q1: Who are the named recipients of the Monday report distribution?  
- Q2: What is the confirmed definition of "margin %" — gross or net?  
- Q3: Is YoY comparison a Phase 2 priority, and if so, what is the target timeline?

---

## Tips

- The messier your notes, the more useful this prompt is — AI handles unclear input well
- Always add your own domain knowledge after the AI draft — it won't know internal system names or company-specific rules
- Use the Open Questions output to drive your very next stakeholder conversation
- Follow up with: *"Now turn the functional requirements into Jira-ready user stories"*
