# Control Phase

## Objective
Ensure improvements are sustained over time through 
monitoring systems, control plans, and standardized 
processes. Prevent regression to previous performance levels.

## Control Plan Overview

| Process | Key Metric | Control Method | Frequency | Owner |
|---------|-----------|----------------|-----------|-------|
| Supplier Management | On-Time Delivery Rate | SPI Scorecard + Power BI | Monthly | Procurement |
| Customer Retention | Churn Rate % | RFM Re-segmentation | Monthly | Marketing |
| Payment Collection | Order to Cash Cycle | AR Aging Review | Monthly | Finance |
| Budget Execution | Budget Variance % | Mid-month Review Gate | Monthly | Finance |
| Quality | OEE %, DPMO | Process Review | Monthly | Operations |
| Inventory | Stockout Rate % | ABC Review | Monthly | Supply Chain |

---

## Control Charts — Key Metrics

### Metric 1 — On-Time Delivery Rate %

| Control Parameter | Value |
|------------------|-------|
| Target | 85% |
| Upper Control Limit (UCL) | 90% |
| Lower Control Limit (LCL) | 80% |
| Current Baseline | 47% |
| Alert Threshold | < 75% after improvement |
| Review Frequency | Monthly |

**Control Action:**
> If On-Time Delivery drops below LCL for 2 consecutive months,
> trigger supplier performance review and escalation process.

---

### Metric 2 — Churn Rate %

| Control Parameter | Value |
|------------------|-------|
| Target | ≤ 25% |
| Upper Control Limit (UCL) | 30% |
| Lower Control Limit (LCL) | 20% |
| Current Baseline | 41% |
| Alert Threshold | > 30% after improvement |
| Review Frequency | Monthly |

**Control Action:**
> If Churn Rate exceeds UCL, activate emergency retention
> campaign and review RFM segmentation immediately.

---

### Metric 3 — Budget Variance %

| Control Parameter | Value |
|------------------|-------|
| Target | ≤ 5% |
| Upper Control Limit (UCL) | 8% |
| Lower Control Limit (LCL) | -3% |
| Current Baseline | +11% |
| Alert Threshold | > 8% |
| Review Frequency | Monthly |

**Control Action:**
> If Budget Variance exceeds UCL, freeze discretionary
> spending and initiate mid-month review within 5 days.

---

### Metric 4 — OEE %

| Control Parameter | Value |
|------------------|-------|
| Target | 85% |
| Upper Control Limit (UCL) | 90% |
| Lower Control Limit (LCL) | 80% |
| Current Baseline | 82% |
| Alert Threshold | < 80% |
| Review Frequency | Monthly |

**Control Action:**
> If OEE drops below LCL, trigger component analysis
> (Availability, Performance, Quality Rate) and
> identify root cause within 48 hours.

---

### Metric 5 — Sigma Level

| Control Parameter | Value |
|------------------|-------|
| Target | 5 Sigma |
| Current Baseline | 4 Sigma |
| DPMO Target | ≤ 233 |
| DPMO Current | 1,106 |
| Alert Threshold | DPMO > 2,000 |
| Review Frequency | Quarterly |

**Control Action:**
> If DPMO exceeds alert threshold, activate DMAIC
> sub-project focused on defect reduction.

---

## Standard Operating Procedures (SOPs)

### SOP 1 — Monthly Supplier Review
| Step | Action | Owner |
|------|--------|-------|
| 1 | Export SPI data from Power BI | Analytics |
| 2 | Review top 10 and bottom 10 suppliers | Procurement |
| 3 | Issue performance improvement notice to suppliers below 60 SPI | Procurement |
| 4 | Update supplier scorecard | Procurement |
| 5 | Escalate suppliers below 50 SPI for contract review | Management |

### SOP 2 — Monthly RFM Review
| Step | Action | Owner |
|------|--------|-------|
| 1 | Refresh RFM segmentation in Power BI | Analytics |
| 2 | Identify customers who moved to At Risk | Marketing |
| 3 | Activate retention offer within 48 hours | Marketing |
| 4 | Review Lost customers for win-back eligibility | Sales |
| 5 | Report retention rate vs target | Management |

### SOP 3 — Monthly Budget Review Gate
| Step | Action | Owner |
|------|--------|-------|
| 1 | Pull Budget vs Actual from Power BI | Finance |
| 2 | Identify departments over 5% variance | Finance |
| 3 | Request variance explanation from department heads | Finance |
| 4 | Approve or freeze additional spend requests | Management |
| 5 | Update forecast for remaining months | Finance |

### SOP 4 — Quarterly Quality Review
| Step | Action | Owner |
|------|--------|-------|
| 1 | Review DPMO and Sigma Level trend | Quality |
| 2 | Analyze Defects by Category — focus on above-median | Quality |
| 3 | Review OEE component breakdown | Operations |
| 4 | Update control limits if process has shifted | Quality |
| 5 | Report to management with improvement actions | Quality |

---

## Power BI as Control System

The Power BI dashboard serves as the primary control
monitoring system for all improvement initiatives.

### Dashboard Usage by Process

| Page | Control Purpose | Review Cadence |
|------|----------------|----------------|
| Executive Overview | Overall health check — all KPIs | Weekly |
| Process Efficiency & Quality | OEE, Sigma, DPMO monitoring | Monthly |
| Sales & Customer | Churn, RFM, Retention monitoring | Monthly |
| Supply Chain & Inventory | Supplier SPI, Delivery monitoring | Monthly |
| Budget & Variance | Budget execution control | Monthly |
| DevOps & Project Tracking | Project improvement tracking | Weekly |

### Automated Alerts (Planned)
| Metric | Alert Condition | Channel |
|--------|----------------|---------|
| On-Time Delivery | < 75% | Email to Procurement |
| Churn Rate | > 30% | Email to Marketing |
| Budget Variance | > 8% | Email to Finance |
| OEE | < 80% | Email to Operations |
| Stockout Rate | > 5% | Email to Supply Chain |

---

## Lessons Learned

| Area | Learning | Action |
|------|----------|--------|
| Data Quality | Delivery date proxy affects accuracy | Implement actual delivery date capture |
| Measurement | TODAY() in DAX causes issues with historical data | Use MAX(Date) for relative calculations |
| Process | Forecasting accuracy (97%) does not prevent overspend | Control must focus on execution, not planning |
| Customer | RFM segmentation requires column, not measure in Power BI | Build calculated columns for segmentation |
| Supplier | All suppliers below target — systemic issue not individual | Framework needed, not case-by-case management |

---

## Project Closure Criteria

| Criterion | Status | Target Date |
|-----------|--------|-------------|
| All 5 improvement actions implemented | 🟡 In Progress | Month 3 |
| KPIs trending toward targets | 🟡 In Progress | Month 6 |
| Control plans documented and active | ✅ Complete | Month 1 |
| SOPs created and communicated | ✅ Complete | Month 1 |
| Power BI dashboard published | 🟡 In Progress | Month 1 |
| GitHub repository documented | ✅ Complete | Month 1 |
| VSM current and future state | 🔴 Planned | Month 2 |

---

## Deliverables — Control Phase
- [x] Control plan for all key metrics
- [x] Control limits defined per metric
- [x] Standard Operating Procedures (4 SOPs)
- [x] Power BI monitoring plan
- [x] Lessons learned documented
- [x] Project closure criteria defined
- [ ] Automated alerts implementation *(planned)*
- [ ] VSM Future State *(planned)*
- [ ] Real data validation *(requires live implementation)*
