# Analyze Phase

## Objective
Identify and validate root causes of the performance gaps 
identified in the Measure phase using data-driven analysis.

## Problem Prioritization — Pareto Analysis

### Top Issues by Business Impact
| Rank | Problem | Impact | Frequency | Priority |
|------|---------|--------|-----------|----------|
| 1 | On-Time Delivery 47% | Revenue & Churn Risk | Every order | Critical |
| 2 | Process Cycle Efficiency 78% | Cost & Speed | Daily | High |
| 3 | At Risk Customers 268 | Revenue Loss | Ongoing | High |
| 4 | OEE 82% vs 85% | Capacity Loss | Daily | Medium |
| 5 | Budget Overspend 11% | Financial Control | Monthly | Medium |

## Root Cause Analysis

### Problem 1 — On-Time Delivery (47%)

#### 5 Whys Analysis — On-Time Delivery 47%

| Why | Question | Answer |
|-----|----------|--------|
| Why 1 | Why is On-Time Delivery only 47%? | More than half of purchase orders arrive after expected date |
| Why 2 | Why do orders arrive late? | Suppliers consistently underperform — SPI avg 41/100 |
| Why 3 | Why do suppliers underperform? | No supplier development program — single source dependency — no SLA enforcement |
| Why 4 | Why is there no supplier management framework? | Procurement lacks performance review gates — selection based on cost only |
| Why 5 | Why is selection cost-focused only? | TCO not used in evaluation — delivery performance not weighted in scorecard |
| **Root Cause** | | **Absence of supplier performance management framework with TCO-based evaluation and SLA enforcement** |

#### Fishbone Diagram (Ishikawa) — On-Time Delivery 47%

| Category | Root Causes |
|----------|------------|
| **Supplier** | SPI avg 41/100 — Single source dependency — No supplier development program — Quality issues |
| **Process** | No SLA enforcement gates — Manual PO process — Long approval time — No escalation path |
| **System** | No real-time tracking — No automated alerts — No KPI dashboard for suppliers |
| **People** | No dedicated supplier manager — No performance reviews — Cost-only evaluation focus |
| **Material** | Stockout 3% — Overstock items — ABC classification not used in ordering |
| **Measurement** | Delivery date is proxy only — No SLA defined — Reactive not proactive monitoring |

### Problem 2 — Process Cycle Efficiency (4%)

#### Value Stream Analysis — Order to Cash Current State

| Process | Cycle Time | OTD / Output |
|------|------|-------------|
| Receive Order | 1h | Uptime: 99% |
| Wait (queue) | 2h | — |
| Check & Pick & Pack | 4h | Uptime: 90% |
| Wait (queue) | 4h | — |
| Ship Order | 30h | OTD: 47% |
| Wait (queue) | 4h | — |
| Invoice | 2h | Uptime: 98% |

**Summary:**

| Metric | Value |
|--------|-------|
| Process Time (PT) | 37h |
| Wait Time | 10h |
| Lead Time (LT) | 47h |
| Process Cycle Efficiency (PCE) | 78.7% |
| Order to Cash Cycle Time | 47h |
| On-Time Delivery Rate % | 47.1% |
| Average Days Outstanding | 47 |
| Churn Rate % | 41% |
| Sigma Level | 4 |
| Supplier Performance Index (SPI) | 41/100 |

**Bottlenecks Identified (Triangle markers in VSM):**

| Issue | Severity | Description |
|-------|----------|-------------|
| Ship Order | 🔴 Critical | -50 throughput; OTD only 47%; backlog accumulating |
| Check & Pick & Pack | 🟡 Medium | -30 throughput; uptime 90% |
| Supplier Performance | 🔴 Critical | SPI 41/100 — Low performance rating |
| Customer Retention | 🟡 Medium | 272 Champions vs 268 At Risk (near 1:1 split) |

#### Order to Cash Cycle Time — 47h

**Root Cause: Ship Order is the primary bottleneck**

| Issue | Impact |
|-------|--------|
| Ship Order has highest cycle time (30h) of all process steps | High |
| OTD at 47% directly tied to Ship Order delays | High |
| Throughput drop of -50 at Ship Order stage | High |
| Backlog flagged specifically at Invoice/Ship handoff | High |
| Supplier SPI 41/100 may be feeding delays upstream | Medium |
| Churn Rate 41% — At Risk segment (268) nearly equals Champions (272) | Medium |

### Problem 3 — Customer Retention (59%)

#### RFM Analysis Findings

| Segment | Count | % of Base | Action |
|---------|-------|-----------|--------|
| Champions | 272 | 28% | Protect and grow |
| Loyal Customers | 186 | 19% | Reward loyalty |
| Need Attention | 115 | 12% | Re-engage |
| At Risk | 268 | 28% | Urgent intervention |
| Lost | 123 | 13% | Win-back campaign |

> **Key Finding:** At Risk (268) ≈ Champions (272)
> The customer base is at a critical tipping point.
> Without intervention, Champions of tomorrow are leaving today.

**Churn Drivers:**

| Driver | Status |
|--------|--------|
| Average Days Since Last Purchase | Increasing |
| Purchase frequency in At Risk segment | Declining |
| Proactive retention program | Not exists |
| Discount strategy targeting At Risk | Not targeted |

### Problem 4 — OEE (82% vs 85% target)

#### OEE Component Breakdown

| Component | Current | Target | Gap | Root Cause |
|-----------|---------|--------|-----|------------|
| Availability | 91% | 95% | -4pp | Unplanned downtime, maintenance gaps |
| Performance | 95% | 98% | -3pp | Speed losses, theoretical vs actual output |
| Quality Rate | 95% | 99% | -4pp | Defects in Sports and Health & Beauty |
| **OEE Total** | **82%** | **85%** | **-3pp** | Combined component gaps |

### Problem 5 — Budget Overspend (11%)

#### Variance Analysis

| Metric | Value |
|--------|-------|
| Total Budget | 165M |
| Total Actual | 183M |
| Variance | +18M (+11%) |
| Forecast Accuracy | 97% ✅ |

> **Key Finding:** Forecast is accurate but execution overspends.
> This indicates a **control gap**, not a planning gap.

**Monthly Variance Pattern:**

| Month | Variance | Status |
|-------|----------|--------|
| May | +19.78% | 🔴 Highest overspend |
| August | +18.52% | 🔴 Second highest |
| Average | +11.01% | 🟡 Consistently above budget |
| December | -0.26% | ✅ Only under-budget month |

**Root Causes:**

| Root Cause | Impact |
|------------|--------|
| No mid-month budget review gates | High |
| Committed spend not monitored vs available budget | High |
| No automated alerts for budget threshold breaches | Medium |

## Correlation Analysis

### On-Time Delivery vs Supplier Performance
Finding: All top 10 suppliers score between 58-66 SPI
No supplier reaches target of 85
This confirms systemic supplier management failure,
not individual supplier issues.

### Defects by Category
Above Median (5.59%):
├── Sports:           6.86% → Priority 1
├── Health & Beauty:  6.64% → Priority 2
└── Food & Beverages: 6.15% → Priority 3
Below Median:
├── Toys:       4.59% → Best performing
└── Electronics: 4.90% → Second best

## Validated Root Causes Summary

| # | Root Cause | Impact | Evidence |
|---|-----------|--------|---------|
| 1 | No supplier performance management framework | On-Time Delivery 47% | SPI avg 41, all suppliers below target |
| 2 | Payment collection process inefficiency | Order to Cash 701 days | AR aging analysis |
| 3 | No customer retention program | Churn 41%, 268 At Risk | RFM segmentation |
| 4 | Availability losses in operations | OEE 82% | Component breakdown |
| 5 | No budget execution control gates | Overspend 11% | Monthly variance pattern |

## Deliverables — Analyze Phase
- [x] Pareto prioritization of problems
- [x] 5 Whys analysis — On-Time Delivery
- [x] Fishbone diagram — On-Time Delivery
- [x] Value Stream Analysis — Order to Cash
- [x] RFM customer analysis
- [x] OEE component breakdown
- [x] Budget variance pattern analysis
- [x] Root causes validated with data
- [ ] VSM Current State map *(visual — planned)*
- [ ] Statistical hypothesis testing *(planned)*