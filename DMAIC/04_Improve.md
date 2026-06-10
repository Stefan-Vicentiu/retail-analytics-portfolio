# Improve Phase

## Objective
Define and implement data-driven improvement solutions 
for the validated root causes identified in the Analyze phase.
Prioritize actions by impact and feasibility.

## Improvement Prioritization Matrix

| # | Improvement Action | Impact | Effort | Priority |
|---|-------------------|--------|--------|----------|
| 1 | Supplier Performance Management Framework | 🔴 High | 🟡 Medium | P1 |
| 2 | Customer Retention Program — At Risk Segment | 🔴 High | 🟢 Low | P1 |
| 3 | Payment Collection Process Improvement | 🔴 High | 🟡 Medium | P1 |
| 4 | Budget Execution Control Gates | 🟡 Medium | 🟢 Low | P2 |
| 5 | OEE Availability Improvement | 🟡 Medium | 🔴 High | P2 |
| 6 | Process Cycle Efficiency — Waste Elimination | 🔴 High | 🔴 High | P3 |

---

## Improvement 1 — Supplier Performance Management

### Problem
On-Time Delivery: 47% vs 85% target
Supplier Performance Index: 41/100 average
All top 10 suppliers score below target (58-66 SPI)

### Solution
Implement a Supplier Performance Management Framework
based on Total Cost of Ownership (TCO) evaluation.

### Action Plan

| Action | Owner | Timeline | KPI Target |
|--------|-------|----------|------------|
| Define SLA for all active suppliers | Procurement | Month 1 | 100% suppliers with SLA |
| Implement monthly SPI scorecard review | Procurement | Month 1 | SPI ≥ 85 for top 20 suppliers |
| Identify and reduce single-source dependencies | Supply Chain | Month 2 | Single Source Risk ≤ 10% |
| Launch supplier development program | Procurement | Month 2 | SPI improvement ≥ 10pp |
| Integrate TCO in supplier selection criteria | Procurement | Month 3 | TCO used in 100% new contracts |
| Automate delivery performance alerts | IT | Month 2 | Real-time SPI dashboard |

### Expected Impact

| Metric | Current | Target | Expected Improvement |
|--------|---------|--------|---------------------|
| On-Time Delivery Rate | 47% | 85% | +38pp over 6 months |
| Supplier Performance Index | 41 | 85 | +44 points |
| Single Source Risk | Unknown | ≤ 10% | Risk reduction |
| Late Deliveries | 53% | ≤ 15% | -38pp |

### Power BI Monitoring
> Track via **Supply Chain & Inventory** page:
> - Supplier Performance Index trend
> - On-Time Delivery Rate by Month
> - Late Deliveries count

---

## Improvement 2 — Customer Retention Program

### Problem
Churn Rate: 41%
At Risk Customers: 268 (28% of base)
Lost Customers: 123 (13% of base)

### Solution
Implement a targeted retention program using RFM 
segmentation to prioritize At Risk customers.

### Action Plan

| Action | Owner | Timeline | KPI Target |
|--------|-------|----------|------------|
| Define retention offers for At Risk segment | Marketing | Month 1 | Offer for all 268 At Risk |
| Launch win-back campaign for Lost customers | Marketing | Month 1 | Recover ≥ 20% of 123 Lost |
| Implement loyalty rewards for Champions | Marketing | Month 1 | Retention ≥ 90% for Champions |
| Set up automated churn risk alerts | CRM/IT | Month 2 | Alert when customer moves to At Risk |
| Monthly RFM re-segmentation review | Analytics | Ongoing | Churn Rate ≤ 25% |
| Targeted discount strategy for At Risk | Sales | Month 1 | Discount ROI positive |

### Expected Impact

| Metric | Current | Target | Expected Improvement |
|--------|---------|--------|---------------------|
| Customer Retention Rate | 59% | 75% | +16pp |
| Churn Rate | 41% | ≤ 25% | -16pp |
| At Risk Customers | 268 | ≤ 100 | -168 customers |
| Lost Customers | 123 | ≤ 60 | -63 customers recovered |

### Power BI Monitoring
> Track via **Sales & Customer** page:
> - RFM Segmentation trend
> - Churn Rate % monthly
> - Customer Retention Rate %

---

## Improvement 3 — Payment Collection Process

### Problem
Order to Cash Cycle Time: 701 days
AR > 90 Days: significant outstanding balance
Collection Effectiveness Index: not optimized

### Solution
Redesign payment collection process with automated 
reminders and AR aging management.

### Action Plan

| Action | Owner | Timeline | KPI Target |
|--------|-------|----------|------------|
| Implement automated payment reminders | Finance/IT | Month 1 | AR 0-30 Days ≥ 60% of total AR |
| Define escalation path for AR > 60 Days | Finance | Month 1 | AR > 90 Days ≤ 10% of total |
| Introduce early payment incentives | Finance | Month 2 | DSO reduction ≥ 30 days |
| Monthly AR aging review process | Finance | Ongoing | CEI ≥ 85% |
| Set credit limits based on payment history | Finance | Month 2 | Bad Debt ≤ 1% of revenue |

### Expected Impact

| Metric | Current | Target | Expected Improvement |
|--------|---------|--------|---------------------|
| Order to Cash Cycle Time | 701 days | ≤ 45 days | -656 days |
| AR > 90 Days | High | ≤ 10% of AR | Significant reduction |
| Days Sales Outstanding (DSO) | High | ≤ 30 days | Cash flow improvement |
| Collection Effectiveness Index | Unknown | ≥ 85% | Measurable improvement |

### Power BI Monitoring
> Track via **Budget & Variance** page:
> - AR aging buckets (0-30, 31-60, 61-90, >90 days)
> - Collection Effectiveness Index trend
> - Days Sales Outstanding monthly

---

## Improvement 4 — Budget Execution Control

### Problem
Budget Variance: +11% consistently
Forecast Accuracy: 97% (strong — not the issue)
Peak overspend: May (+19.78%), August (+18.52%)

### Solution
Implement monthly budget execution gates with 
automated threshold alerts.

### Action Plan

| Action | Owner | Timeline | KPI Target |
|--------|-------|----------|------------|
| Define budget variance threshold alerts (±5%) | Finance | Month 1 | Alert on all breaches |
| Implement mid-month budget review meetings | Finance | Month 1 | Monthly cadence |
| Monitor Committed Amount vs Available Budget | Finance | Ongoing | Utilization ≤ 95% |
| Investigate May and August overspend drivers | Finance | Month 1 | Root cause documented |
| Introduce budget freeze process above 10% variance | Finance | Month 2 | Variance ≤ 5% |

### Expected Impact

| Metric | Current | Target | Expected Improvement |
|--------|---------|--------|---------------------|
| Budget Variance | +11% | ≤ 5% | -6pp |
| Months over budget | 11 of 12 | ≤ 3 of 12 | Controlled execution |
| Available Budget monitoring | Reactive | Proactive | Real-time visibility |

### Power BI Monitoring
> Track via **Budget & Variance** page:
> - Budget Variance % by Month trend
> - Available Budget vs Committed Amount
> - Over Budget Count

---

## Improvement 5 — OEE Availability Improvement

### Problem
OEE: 82% vs 85% target
Availability: 91% vs 95% target (primary gap)
Quality Rate: 95% with Sports and Health & Beauty above median

### Solution
Implement preventive maintenance schedule and 
category-specific quality improvement programs.

### Action Plan

| Action | Owner | Timeline | KPI Target |
|--------|-------|----------|------------|
| Analyze downtime causes by category | Operations | Month 1 | Root cause per category |
| Implement preventive maintenance schedule | Operations | Month 2 | Availability ≥ 93% |
| Quality improvement focus on Sports category | Quality | Month 1 | DPU Sports ≤ 5% |
| Quality improvement focus on Health & Beauty | Quality | Month 1 | DPU H&B ≤ 5% |
| Monthly OEE review with component breakdown | Operations | Ongoing | OEE ≥ 85% |

### Expected Impact

| Metric | Current | Target | Expected Improvement |
|--------|---------|--------|---------------------|
| OEE % | 82% | 85% | +3pp |
| Availability | 91% | 95% | +4pp |
| Sports DPU | 6.86% | ≤ 5% | -1.86pp |
| Health & Beauty DPU | 6.64% | ≤ 5% | -1.64pp |

### Power BI Monitoring
> Track via **Process Efficiency & Quality** page:
> - OEE Gauge vs 85% target
> - Defects by Category
> - First Pass Yield % trend

---

## Improvement Roadmap

| Month | Priority Actions |
|-------|----------------|
| Month 1 | Supplier SLA definition, At Risk retention campaign, AR automated reminders, Budget alerts setup |
| Month 2 | Supplier development program, Win-back campaign, TCO integration, Mid-month budget reviews |
| Month 3 | Single source risk reduction, OEE preventive maintenance, CEI monitoring |
| Month 4-6 | Monitor KPIs, adjust programs, measure improvement vs baseline |

## Expected Total Business Impact

| Area | Current | Target | Business Value |
|------|---------|--------|---------------|
| On-Time Delivery | 47% | 85% | Customer satisfaction & retention |
| Churn Rate | 41% | ≤ 25% | Revenue protection |
| Order to Cash | 701 days | ≤ 45 days | Cash flow improvement |
| Budget Variance | +11% | ≤ 5% | Cost control |
| OEE | 82% | 85% | Capacity & quality improvement |
| Sigma Level | 4 | 5 | Quality maturity advancement |

## Deliverables — Improve Phase
- [x] Improvement prioritization matrix
- [x] Action plans for top 5 improvements
- [x] Expected impact quantified per improvement
- [x] Power BI monitoring linkage defined
- [x] Implementation roadmap
- [ ] VSM Future State map *(planned)*
- [ ] Pilot implementation results *(real data needed)*
- [ ] Cost-Benefit Analysis *(planned)*
