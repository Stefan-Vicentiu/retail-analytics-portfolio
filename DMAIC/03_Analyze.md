# Analyze Phase

## Objective
Identify and validate root causes of the performance gaps 
identified in the Measure phase using data-driven analysis.

## Problem Prioritization — Pareto Analysis

### Top Issues by Business Impact
| Rank | Problem | Impact | Frequency | Priority |
|------|---------|--------|-----------|----------|
| 1 | On-Time Delivery 47% | Revenue & Churn Risk | Every order | Critical |
| 2 | Process Cycle Efficiency 4% | Cost & Speed | Daily | Critical |
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

#### Value Stream Analysis
Order to Cash Process — Current State
Customer Order → [WAIT 48h] → Order Processing → [WAIT] →
Warehouse Pick → [WAIT] → Quality Check → [WAIT] →
Dispatch → [WAIT] → Delivery → Invoice → [WAIT 701 days] →
Payment Collection
Value-Added Time:    2 hours  (4%)
Non-Value-Added:    46 hours  (96%)
Total Cycle Time:   48 hours
Waste Categories Identified (7 Wastes — Lean):
├── Waiting:     Major — between each process step
├── Transport:   Medium — multiple warehouse touchpoints
├── Inventory:   Medium — overstock items identified
├── Defects:     Medium — 5.26% avg DPU
├── Processing:  Minor — manual approval steps
├── Motion:      Minor — warehouse layout
└── Overproduction: Low — demand forecasting gap

#### Order to Cash Cycle Time — 701 Days
Root Cause: Payment collection process is the primary driver
├── Outstanding invoices aging beyond 90 days
├── No automated payment reminder system
├── AR 0-30 Days vs AR >90 Days ratio not optimized
└── Collection Effectiveness Index not monitored

### Problem 3 — Customer Retention (59%)

#### RFM Analysis Findings
Customer Segmentation:
├── Champions:      272 (28%) — protect and grow
├── Loyal:          186 (19%) — reward loyalty
├── Need Attention: 115 (12%) — re-engage
├── At Risk:        268 (28%) — urgent intervention
└── Lost:           123 (13%) — win-back campaign
Key Finding: At Risk (268) ≈ Champions (272)
This indicates the customer base is at a critical
tipping point — without intervention,
Champions of tomorrow are leaving today.
Churn Drivers:
├── Average Days Since Last Purchase increasing
├── Purchase frequency declining in At Risk segment
├── No proactive retention program identified
└── Discount strategy not targeted to At Risk segment

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
Total Budget:  165M
Total Actual:  183M
Variance:      +18M (+11%)
Forecast Accuracy: 97% ✅
Finding: Forecast is accurate but execution overspends.
This indicates a control gap, not a planning gap.
Monthly Pattern:
├── May: +19.78% — highest overspend month
├── August: +18.52% — second highest
├── December: -0.26% — only under-budget month
└── Average: +11.01% consistently above budget
Root Cause:
├── No mid-month budget review gates
├── Committed spend not monitored vs available budget
└── No automated alerts for budget threshold breaches

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
