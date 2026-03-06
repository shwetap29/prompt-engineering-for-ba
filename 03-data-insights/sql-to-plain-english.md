# 🔤 SQL to Plain English

**Level:** Intermediate  
**Category:** Data Insights  
**Time Saved:** 15–20 min per query explanation

---

## What This Is

A prompt that translates a SQL query into a plain-language explanation that any non-technical stakeholder can understand — and also helps you explain what the data is actually showing.

---

## When to Use It

- When a developer or analyst shares a SQL query and you need to understand or explain it
- When writing documentation for a report and you need to describe the logic in business terms
- When a stakeholder asks "how is this number calculated?" and you need a clear answer fast

---

## The Prompt — Explain a SQL Query

```
You are a Business Analyst who is excellent at translating technical 
database queries into plain business language.

Explain the following SQL query in simple terms that a non-technical 
Finance or Business stakeholder could understand.

Your explanation should answer:
1. What data is this query pulling — what is the result set?
2. Where is the data coming from — what tables or sources?
3. What filters or conditions are applied?
4. What calculations or transformations are happening?
5. In one sentence: what business question does this query answer?

SQL Query:
[PASTE YOUR SQL HERE]

Audience: non-technical business user
Format: use the 5 numbered questions as headers, keep each answer to 2–3 sentences max
```

---

## Filled Example

**Your input:**
```sql
SELECT 
    r.region_name,
    SUM(o.order_value) AS total_revenue,
    COUNT(DISTINCT o.customer_id) AS unique_customers,
    SUM(o.order_value) / COUNT(DISTINCT o.customer_id) AS avg_order_value
FROM orders o
JOIN regions r ON o.region_id = r.region_id
WHERE o.order_date >= '2026-01-01'
  AND o.order_date < '2026-02-01'
  AND o.status = 'completed'
GROUP BY r.region_name
ORDER BY total_revenue DESC
```

**AI Output:**

---

**1. What data is this pulling?**  
This query produces a summary table showing revenue, customer count, and average order value — broken down by sales region, for a specific time period.

**2. Where does the data come from?**  
It combines two tables: the `orders` table (which holds individual transaction records) and the `regions` table (which maps each order to a named region).

**3. What filters are applied?**  
Only orders from January 2026 are included, and only orders with a status of "completed" — so cancelled, pending, or refunded orders are excluded from all calculations.

**4. What calculations are happening?**  
For each region, the query totals the order values (revenue), counts distinct customers (so a customer with multiple orders is only counted once), and divides revenue by unique customers to get the average spend per customer.

**5. In one sentence: what business question does this answer?**  
"How did each sales region perform in January 2026, in terms of total revenue, customer reach, and average customer spend?"

---

## Bonus Prompt — Write SQL from a Business Description

```
You are a SQL developer working with a Business Analyst.

Write a SQL query that answers the following business question. 
Use clear, readable formatting with comments explaining each section.

Business question:
[DESCRIBE WHAT DATA YOU NEED IN PLAIN LANGUAGE]

Available tables and columns (describe what you know):
[LIST YOUR TABLES AND KEY COLUMNS, OR PASTE YOUR SCHEMA]

Database type: [e.g., SQL Server / PostgreSQL / MySQL / BigQuery]
```

---

## Tips

- This prompt is excellent for documenting report logic — paste the explanation into your BRD or report spec
- If AI's explanation of the SQL is unclear, follow up: *"Explain step 4 in simpler terms"*
- Use the bonus prompt when building quick-turn ad hoc queries — always review and test before using in production
