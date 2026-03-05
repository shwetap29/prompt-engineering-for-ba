# 📝 User Story Generator

**Level:** Intermediate  
**Category:** Requirements  
**Time Saved:** 30–40 min per feature

---

## What This Is

A prompt that converts a feature request or business need into properly formatted Agile user stories with acceptance criteria — ready to paste directly into Jira.

---

## When to Use It

- During sprint planning or backlog grooming
- When a stakeholder gives you a request and you need to break it into dev-ready tickets
- When you have a BRD requirement and need to convert it into user stories

---

## The Prompt

```
You are a Business Analyst writing Agile user stories for a development team.

Convert the business requirement below into 3–5 user stories.

Use the standard format for each:
"As a [user type], I want [action], so that [benefit]."

For each user story also provide:
- 3–4 acceptance criteria in Gherkin format: Given / When / Then
- A suggested story point estimate (1, 2, 3, 5, or 8) with a one-line reason
- Any edge cases or dependencies to flag

Business Requirement:
[PASTE YOUR REQUIREMENT HERE]

User types involved (if known): [e.g., Admin, Manager, Standard User]
Any technical constraints to keep in mind: [or write "none known"]
```

---

## Filled Example

**Your input:**
```
The marketing team needs to export campaign performance data from the 
dashboard as a CSV file, with filters for date range and campaign name.
```

**AI Output:**

---

**User Story 1**  
As a Marketing Manager, I want to export campaign data as a CSV file, so that I can analyse performance in Excel without manually copying data.  
*Story Points: 3 — standard export, no complex data transformation required*

**Acceptance Criteria:**
- Given I am on the Campaign Dashboard, When I click "Export to CSV", Then a CSV file downloads to my device within 10 seconds
- Given I have applied a date range filter, When I export, Then the CSV contains only data within that date range
- Given the export contains more than 10,000 rows, Then a progress indicator is shown and the file completes within 60 seconds

**Edge Case:** What should happen if no data exists for the selected filters — download an empty CSV or show a "no data" message?

---

**User Story 2**  
As a Marketing Analyst, I want to filter the export by campaign name, so that I can analyse one campaign's performance in isolation.

**Acceptance Criteria:**
- Given I type a campaign name in the filter, When I click Export, Then only rows matching that campaign appear in the CSV
- Given I clear the campaign name filter, When I export, Then all campaigns are included
- Given no campaigns match my search term, Then a "no matching campaigns found" message is shown before export

*Story Points: 2 — filter already exists, export simply needs to respect it*

---

## Tips

- Provide user types upfront — stories become much more targeted
- If stories feel too broad, follow up: *"Break User Story 1 into two smaller stories"*
- The edge cases AI flags often become your best UAT test scenarios
- Follow up with: *"Now write UAT test cases for User Story 1"*
