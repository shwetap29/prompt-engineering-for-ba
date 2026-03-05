# ✅ Acceptance Criteria Reviewer

**Level:** Intermediate  
**Category:** Requirements  
**Time Saved:** 20–30 min per story

---

## What This Is

A prompt that reviews your acceptance criteria for three things that matter most: clarity, testability, and completeness. AI returns specific feedback and rewrites any weak criteria.

---

## When to Use It

- Before submitting user stories to the development team
- As a self-review step before stakeholder sign-off
- When AC was written by a developer or product manager and you want to QA it

---

## The Prompt

```
You are a senior QA-focused Business Analyst reviewing acceptance criteria 
before sprint planning.

Review the user story and acceptance criteria below. For each criterion, 
assess:

1. Clarity — is it specific and unambiguous? Flag any vague words like 
   "fast", "easy", "user-friendly", "appropriate"

2. Testability — can it be objectively tested with a clear pass or fail? 
   If not, explain why

3. Completeness — what is missing? Look specifically for:
   - Negative cases (what happens when something goes wrong?)
   - Permission/role cases (does behaviour differ by user type?)
   - Edge cases (empty data, maximum limits, unusual inputs)

4. Rewrite — for any weak criterion, provide an improved version

User Story:
[PASTE USER STORY]

Acceptance Criteria:
[PASTE ACCEPTANCE CRITERIA — one per line]
```

---

## Filled Example

**Your input:**

> *User Story:* As an Admin, I want to deactivate user accounts so that unauthorised users can no longer access the system.
>
> *AC1:* The admin should be able to deactivate accounts easily.  
> *AC2:* The user gets an email notification.  
> *AC3:* The system should handle this quickly.

**AI Output:**

---

**AC1 — "easily" is vague and not testable**  
❌ Issue: "Easily" is subjective and cannot be measured in a test.  
✅ Rewrite: *"Given the Admin is on the User Management page, When they click 'Deactivate' next to a user record and confirm the prompt, Then the account status changes to 'Inactive' immediately and is reflected on screen."*

**AC2 — partially testable, but incomplete**  
⚠️ Issue: "Gets an email" doesn't specify timing, content, or recipient edge cases.  
✅ Rewrite: *"Given an account is deactivated, When the action is confirmed, Then the affected user receives an email notification within 5 minutes containing their name and a support contact link."*

**AC3 — "quickly" is not testable**  
❌ Issue: "Quickly" has no measurable definition.  
✅ Rewrite: *"The deactivation action completes and the updated status is displayed within 3 seconds of confirmation."*

**Missing Scenarios:**
- What happens if an Admin tries to deactivate their own account? (should be blocked)
- What if the user is currently logged in when deactivated — are they immediately logged out?
- Can a non-Admin user see or access the Deactivate button? (permissions case)

---

## Tips

- Run this review before every sprint planning — it catches problems before they reach development
- The missing scenarios AI identifies are directly usable as UAT test cases
- If AC was developer-written, this prompt is great for translating technical language into business-readable criteria
