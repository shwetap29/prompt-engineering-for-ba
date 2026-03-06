# 🗒️ Meeting Summary Generator

**Level:** Beginner–Intermediate  
**Category:** Stakeholder Communication  
**Time Saved:** 20–30 min per meeting

---

## What This Is

A prompt that converts messy meeting notes — or a raw transcript — into a clean, professional summary with decisions, action items, and owners, ready to send to stakeholders within minutes.

---

## When to Use It

- After any requirements gathering, sprint planning, or stakeholder review call
- When you need to circulate minutes within 24 hours
- When multiple teams attended and clarity on decisions and owners is critical

---

## The Prompt

```
You are a Business Analyst writing a professional meeting summary to send 
to project stakeholders.

Based on the notes or transcript below, write a structured meeting summary 
that includes:

1. Meeting Overview — one line: purpose, date, attendees
2. Key Discussion Points — 3–5 bullet points of what was discussed
3. Decisions Made — numbered list of confirmed decisions only 
   (not things that were discussed, only things that were agreed)
4. Action Items — a table with columns: Action | Owner | Due Date
   (write "TBD" if not mentioned — do not invent a due date)
5. Open Questions / Parking Lot — things raised but not resolved
6. Next Steps — what happens after this meeting

Raw Notes:
[PASTE YOUR NOTES OR TRANSCRIPT HERE]

Tone: professional, factual, neutral — no opinions or interpretations beyond what was said
```

---

## Filled Example

**Your raw notes:**
```
Called with Sarah (PM), three devs, and the client rep (Marcus). They 
want the report live by end of month. Dev said they need the field mapping 
doc first — Sarah will send it by Friday. Marcus said margins should show 
as % not $. UAT dates not confirmed yet. We're all meeting again Thursday.
```

**AI Output:**

---

**Meeting Overview**  
Requirements alignment call | [Date] | Attendees: Sarah (PM), Development Team (x3), Marcus (Client Representative)

**Key Discussion Points**
- Report delivery target confirmed as end of current month
- Development team flagged dependency on field mapping document before build can begin
- Client confirmed preferred format for margin display
- UAT scheduling raised but not yet confirmed

**Decisions Made**
1. Margin figures will display as percentage (%) in the final report — not dollar value
2. Development work will not begin until the field mapping document is received

**Action Items**
| Action | Owner | Due Date |
|---|---|---|
| Send field mapping document to dev team | Sarah | Friday |
| Confirm UAT start and end dates | TBD | Before Thursday call |

**Open Questions**
- Who is responsible for confirming UAT dates — BA, PM, or client?
- Is there a specific template or format required for the field mapping document?

**Next Steps**
- Follow-up call scheduled for Thursday
- BA to follow up on UAT dates before then

---

## Tips

- If you have a Teams or Zoom transcript, paste it directly — AI handles long, messy text well
- Always verify owners and dates before sending — AI sometimes infers these if not explicitly stated
- Add a personal "BA Notes" section at the bottom for follow-ups only you need to track
- Send the summary within 24 hours — the sooner it goes out, the more useful it is
