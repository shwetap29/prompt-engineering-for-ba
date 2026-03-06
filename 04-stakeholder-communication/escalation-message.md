# 🚨 Escalation Message

**Level:** Intermediate  
**Category:** Stakeholder Communication  
**Time Saved:** 20–25 min (plus a lot of stress)

---

## What This Is

A prompt that drafts a professional escalation message when a blocker, risk, or unresolved issue needs to go to leadership — clearly, calmly, and with a proposed path forward rather than just "we need help."

---

## When to Use It

- A dependency is overdue and is now putting a milestone at risk
- A decision hasn't been made and the team is blocked
- A scope change has been introduced informally without proper approval
- Normal follow-up hasn't worked and you need to go up the chain

---

## The Prompt

```
You are a Business Analyst drafting a professional escalation message 
to a senior stakeholder or project sponsor.

The message should:
1. State the issue clearly and factually — no blame, no emotional language
2. Explain the business impact if it stays unresolved (timeline, quality, or cost risk)
3. State specifically what has already been done to resolve it
4. Make a specific, actionable ask — not just "we need your help"
5. Stay under 150 words

Issue: [describe what the problem is]
Business impact if unresolved: [describe the risk — timeline slip, delivery quality, etc.]
What's been tried already: [list the steps you've taken]
Specific ask: [exactly what you need from this person]
Channel: [Email / Slack / Teams]
Tone: calm, factual, solution-focused — not frustrated or accusatory
```

---

## Filled Example

**Your input:**
```
Issue: IT has not provided database access credentials despite two requests 
over 10 days.
Impact: Dev team can't start the data layer — UAT is now at risk of 
slipping by a week.
Already tried: emailed IT helpdesk twice (March 1 and March 6), raised 
in standup.
Ask: IT Manager approves and expedites access for [developer name] by Wednesday.
Channel: Email
```

**AI Output:**

---

**Subject:** Escalation: Database Access Credentials — CRM Dashboard

Hi [IT Manager's name],

I'm writing to escalate an outstanding access request that is now affecting our delivery timeline.

We submitted two helpdesk requests for database read access (March 1 and March 6) for the CRM Dashboard project. After 10 days with no resolution, the development team is unable to begin the data layer build — putting our March 15 UAT start date at risk of a one-week slip.

Could you help expedite this with your team? Specifically, we need read-only access to [database name] provisioned for [developer name] by Wednesday, March 12.

I'm happy to provide any additional details needed. Thank you for your support.

[Your name]

---

## Tips

- Always document what you've already tried — it shows diligence and protects you in writing
- Propose a *specific* resolution (name, date, access level) not just "please look into this"
- CC your own manager if the issue has been unresolved for 2+ weeks
- Pair the written message with a direct conversation wherever possible — escalations land better in combination
