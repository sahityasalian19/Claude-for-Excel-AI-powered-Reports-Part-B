# Claude-for-Excel-AI-powered-Reports-Part-B

# 📊 Part B — Pivot Table Reports | SkyTrail Vacations

> **Project:** Tourism Booking Data Analysis  
> **Company:** SkyTrail Vacations *(fictional dataset)*  
> **Dataset:** 966 rows | 22 columns | Cleaned in Part A  
> **Tool Used:** Microsoft Excel | Claude AI (Anthropic)  
> **Approach:** Role-based prompting — Claude acted as Senior Data Analyst and built reports autonomously

---

## 🔄 How This Phase Is Different

In **Part A (Data Cleaning)**, I handed Claude the data and let it do the cleaning itself.

In **Part B (Reporting)**, I handed Claude the data and let it build the report itself.

> My role shifted from *builder* → *director* → *reviewer*.

This was an intentional experiment to understand what changes when AI executes, not just advises.

---

## 🤖 The Role-Based Prompt Used

```
You are a Data Analyst specializing in Excel reporting and business intelligence.

Your task is to analyze a cleaned dataset and create meaningful pivot table 
reports that surface key business insights. I'm uploading an Excel file, refer Cleaned Data sheet.

Guidelines:
Prioritize reports that show revenue, volume, trends, and comparisons
Use plain language to describe what each pivot table shows
If a calculation is needed (e.g. average, count, sum), state which aggregation you're using and why
Flag any data limitations that may affect the report

Dataset context:
966 rows of cleaned tourism booking data for SkyTrail Vacations.
Columns: Booking ID, Gender, City of Origin, Destination, Package Type,
Accommodation Type, Num Travelers, Final Price INR, Booking Channel,
Payment Method, Booking Status, Customer Rating, Booking Year, Age Group

Focus on: Revenue analysis, booking behavior, customer demographics, 
and package performance.

Your output for each pivot table should include:
1. Report name
2. Rows / Columns / Values / Filters used
3. A short summary of what the report reveals
```
---

## 📋 Reports Built (11 Pivot Tables | 4 Sheets)

### 💰 Sheet 1 — Revenue Analysis

| # | Report Name | Rows | Columns | Values | Key Question |
|---|-------------|------|---------|--------|--------------|
| PT1 | Revenue by Package | Package Type | — | SUM Revenue, COUNT Bookings, AVG Revenue | Which package drives the most revenue? |
| PT2 | Revenue by Destination | Destination | — | SUM Revenue, COUNT Bookings, AVG Revenue | Which destinations are top earners? |

---

### 📋 Sheet 2 — Booking Behaviour

| # | Report Name | Rows | Columns | Values | Key Question |
|---|-------------|------|---------|--------|--------------|
| PT3 | Booking Status by Package | Package Type | — | Booking Status, COUNT Bookings | Which packages have the most cancellations? |
| PT4 | Revenue by Year | Booking Year | — | SUM Revenue, COUNT Bookings, AVG Revenue | How has revenue trended year-over-year? |
| PT5 | Revenue by Payment Method | Payment Method | — | SUM Revenue, COUNT Bookings, AVG Revenue | How do customers prefer to pay? |
| PT6 | Revenue by Booking Channel | Booking Channel | — | SUM Revenue, COUNT Bookings, AVG Revenue | Which channel brings the most business? |

---

### 👥 Sheet 3 — Customer Demographics

| # | Report Name | Rows | Columns | Values | Key Question |
|---|-------------|------|---------|--------|--------------|
| PT7 | Gender × Package | Package Type | Gender | COUNT Bookings | How does gender preference vary by package? |
| PT8 | Bookings by City of Origin | City of Origin | — | SUM Revenue, COUNT Bookings, AVG Revenue | Which cities generate the most bookings? |
| PT9 | Revenue by Age Group | Age Group | — | SUM Revenue, COUNT Bookings, AVG Revenue | Which age segment spends the most? |

---

### 🎯 Sheet 4 — Package Performance

| # | Report Name | Rows | Columns | Values | Key Question |
|---|-------------|------|---------|--------|--------------|
| PT10 | Revenue by Accommodation Type | Accommodation Type | — | SUM Revenue, COUNT Bookings, AVG Revenue | What accommodation type brings in the most? |
| PT11 | Avg Rating by Package | Package Type | — | AVG Customer Rating, COUNT Bookings | Which packages satisfy customers the most? |

---

## 💡 Key Observations (Claude-Generated, Human-Verified)

- **Group Tour** leads all packages in total revenue
- **Maldives** is the top-earning destination by a significant margin
- **55+ age group** dominates both booking volume and revenue — counter-intuitive for a travel brand
- **Adventure & Luxury** packages have the highest cancellation counts
- **3-star hotels** drive more revenue than premium accommodation — suggesting value-conscious travelers
- All packages cluster between **3.7–3.8 average rating** — no clear standout or underperformer
- **Travel Agent** channel outperforms online/walk-in — indicates a trust-driven customer base

---

## 🧠 What I Learned From This Workflow

| Aspect | Phase 1 (I built, Claude assisted) | Phase 2 (Claude built, I directed) |
|--------|-------------------------------------|--------------------------------------|
| My role | Builder + decision maker | Director + reviewer |
| Effort | High execution effort | High thinking effort |
| Errors caught | Power Query UI limitations, age grouping logic | Aggregation choices, field name mismatches |
| Skill developed | Hands-on Power Query & Excel | Prompt engineering + output validation |

> **Takeaway:** Even when AI executes the work, domain knowledge is non-negotiable.  
> You can't validate what you don't understand.

---

## 🛠️ Tools & Technologies

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-F2C811?style=flat&logo=microsoft&logoColor=black)
![Claude AI](https://img.shields.io/badge/Claude_AI-Anthropic-orange?style=flat)

---

## 👤 About

**Sahitya** — QA professional transitioning into Data Analytics  
Building a public portfolio to document the journey.

---
