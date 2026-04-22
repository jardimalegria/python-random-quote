# Startup Financial Modeling (3–5 Year Framework)

This template is designed for early-stage startups that need:
- Board-ready operating plans
- Investor-friendly fundraising forecasts
- Scenario-driven cash/runway management

---

## 1) Model Architecture

Build one integrated model with three linked tabs (or sections):
1. **Assumptions** (single source of truth)
2. **Operating Model** (revenue, costs, hiring)
3. **Financial Statements** (P&L, cash flow, runway, metrics)

### Time Horizon
- **Years 1–2:** monthly periods
- **Year 3:** quarterly periods
- **Years 4–5:** annual periods

---

## 2) Revenue Model (Cohort-Based)

Use customer cohorts to make retention/churn explicit.

### Core Formulas
- **MRR(t)** = Σ over cohorts \[customers retained in month *t* × ARPU(t)\]
- **ARR(t)** = MRR(t) × 12

### Required Inputs
- New customers acquired per month
- Retention curve by cohort age (month 1, 2, …)
- ARPU by plan/tier
- Expansion, contraction, and churn assumptions
- Payment terms (monthly/annual prepay mix)

### SaaS Mechanics (Recommended Layout)
For each month:
- Beginning MRR
- + New MRR
- + Expansion MRR
- − Contraction MRR
- − Churned MRR
- = Ending MRR

Then:
- **Net New MRR** = Ending MRR − Beginning MRR
- **MRR Growth %** = Net New MRR / Beginning MRR

---

## 3) Cost Structure

Split costs into fixed vs. variable and direct vs. indirect.

### COGS (variable-heavy)
- Hosting/infrastructure
- Payment processing
- Variable support costs
- Per-customer third-party tooling

### Operating Expense Buckets
- **Sales & Marketing (S&M):** paid acquisition, sales comp, tools
- **R&D:** engineering, product, design, dev infra
- **G&A:** leadership, legal, finance, HR, insurance, facilities

### Useful Modeling Conventions
- COGS as % of revenue (with scale-based improvement)
- CAC by channel and blended CAC
- Department budgets tied to headcount + tooling + programs
- Add a 10–20% contingency line for unexpected spend

---

## 4) Headcount Plan

Create a role-based hiring schedule by month.

### Inputs
- Start-of-period headcount by role
- Planned hires by month and role
- Attrition assumption (annual)
- Ramp-to-productivity assumption (especially sales)

### Fully-Loaded Compensation
- **Fully loaded cost** = cash compensation × load factor
- Typical load factor: **1.30–1.40** (benefits, taxes, overhead)

### Typical Early-Stage SaaS Mix (Guide)
- Engineering: 40–50%
- Sales & Marketing: 25–35%
- G&A: 10–15%
- Customer Success/Support: 5–10%

---

## 5) Cash Flow and Runway

Revenue and cash are not the same; model timing explicitly.

### Monthly Cash Waterfall
- Beginning cash
- + Cash inflows (collections, financing)
- − Cash outflows (opex, capex, debt service)
- = Ending cash

### Burn and Runway
- **Net burn** = cash outflows − cash inflows (excluding financing)
- **Runway (months)** = current cash / average monthly net burn

If ending cash drops below zero:
- Flag funding gap month
- Size required raise to reach next milestone + 6-month buffer

---

## 6) Core Startup Metrics

### Growth Metrics
- MRR / ARR and growth rates (MoM, YoY)
- Net revenue retention (NRR)
- Gross revenue retention (GRR)

### Unit Economics
- CAC = S&M acquisition spend / new customers
- LTV = ARPU × gross margin % × customer lifetime
- CAC payback period (months)
- LTV/CAC ratio

### Efficiency Metrics
- Burn multiple = net burn / net new ARR
- Magic number = annualized net new ARR / prior-quarter S&M spend
- Rule of 40 = growth % + EBITDA margin %

---

## 7) Scenario Planning (P10 / P50 / P90)

Model three scenarios using the same structure with different assumptions.

### Conservative (P10)
- Slower acquisition
- Lower conversion / pricing
- Higher churn
- Longer sales cycles

### Base (P50)
- Most likely operating assumptions
- Primary board plan

### Optimistic (P90)
- Faster GTM execution
- Better retention and expansion
- Improved CAC efficiency

### Stress Variables (Typical Ranges)
- Acquisition: ±30%
- Churn: ±20%
- ACV/ARPU: ±15%
- CAC: ±25%

---

## 8) Fundraising Layer

Integrate financing rounds directly into cash projections.

### Dilution Math
- Post-money valuation = pre-money + new capital
- Dilution % = new capital / post-money

### Use of Funds Template
- Product/R&D
- GTM (Sales & Marketing)
- G&A/operations
- Working capital buffer

Plan to raise enough to:
1. Reach the next meaningful value-creation milestone
2. Maintain a minimum 6-month post-milestone cash buffer

---

## 9) Validation Checklist

Before sharing the model:
- Growth assumptions are achievable for stage and motion
- Gross margin matches business model norms
- CAC payback and LTV/CAC are plausible
- Headcount and revenue-per-employee trajectory are realistic
- Burn multiple trends toward stronger efficiency over time
- Cash runway is resilient in conservative scenario

---

## 10) Quick Build Sequence

1. Define business model and pricing logic
2. Build cohort-based revenue engine
3. Add cost model (COGS + opex buckets)
4. Add role-level hiring plan
5. Build cash waterfall and runway alerts
6. Layer key SaaS/startup efficiency metrics
7. Clone assumptions for P10/P50/P90 scenarios
8. Add fundraising rounds and dilution outputs
9. Run sanity checks and peer benchmark review

---

## Recommended Worksheet Tabs (Spreadsheet)

1. `Assumptions`
2. `Cohorts_Revenue`
3. `Headcount`
4. `Opex_COGS`
5. `P&L`
6. `CashFlow_Runway`
7. `Metrics`
8. `Scenarios_P10_P50_P90`
9. `Fundraising_Dilution`

This structure keeps assumptions auditable and allows rapid scenario updates for board and investor conversations.
