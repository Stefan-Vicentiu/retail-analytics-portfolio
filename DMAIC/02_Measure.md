# Measure Phase

## Objective
Establish baseline performance metrics to quantify 
the current state of key processes and validate 
the measurement system.

## Data Collection Plan
| Metric | Source | Period | Frequency |
|--------|--------|--------|-----------|
| On-Time Delivery Rate | FACT_Purchases | 2023-2025 | Daily |
| OEE % | FACT_Inventory + FACT_Sales | 2023-2025 | Daily |
| DPMO / Sigma Level | FACT_Sales | 2023-2025 | Monthly |
| Customer Retention Rate | FACT_Sales | 2023-2025 | Monthly |
| Budget Variance | FACT_Budget | 2023-2025 | Monthly |
| Process Cycle Efficiency | FACT_Sales | 2023-2025 | Daily |

## Baseline Performance

### Process Quality Metrics
| Metric | Baseline | Target | Gap |
|--------|----------|--------|-----|
| Sigma Level | 4 | 6 | -2 levels |
| DPMO | 1,106 | 233 | -873 |
| First Pass Yield | 94% | 95% | -1pp |
| OEE % | 82% | 85% | -3pp |
| Availability | 91% | 95% | -4pp |
| Performance | 95% | 98% | -3pp |
| Quality Rate | 95% | 99% | -4pp |

### Delivery Performance Metrics
| Metric | Baseline | Target | Gap |
|--------|----------|--------|-----|
| On-Time Delivery Rate | 47% | 85% | -38pp |
| Supplier Performance Index | 41/100 | 85/100 | -44 |
| Average Delivery Delay | Variable | ≤ 3 days | TBD |
| Stockout Rate | 3% | ≤ 2% | -1pp |
| Inventory Turnover Ratio | 304 | Calibrate | TBD |

### Customer Metrics
| Metric | Baseline | Target | Gap |
|--------|----------|--------|-----|
| Customer Retention Rate | 59% | 75% | -16pp |
| Churn Rate | 41% | ≤ 25% | -16pp |
| Champions Segment | 272 customers | ≥ 40% of base | TBD |
| At Risk Segment | 268 customers | ≤ 10% of base | Critical |
| Lost Customers | 123 customers | Minimize | Critical |

### Financial Metrics
| Metric | Baseline | Target | Gap |
|--------|----------|--------|-----|
| Total Sales | 278M | Growth YoY | TBD |
| Gross Profit Margin | 54% | ≥ 55% | -1pp |
| Budget Variance | +11% | ≤ 5% | -6pp |
| Forecast Accuracy | 97% | ≥ 95% | ✅ Exceeds |
| Process Cycle Efficiency | 4% | ≥ 15% | -11pp |

### Process Efficiency Metrics
| Metric | Baseline | Target | Gap |
|--------|----------|--------|-----|
| Order to Cash Cycle Time | 701 days | ≤ 30 days | Critical |
| Value-Added Time | 2 hours | Maximize | Critical |
| Total Cycle Time | 47 hours | Minimize | TBD |
| Process Cycle Efficiency | 78% | ≥ 89% | -11pp |

## Measurement System Analysis

### Data Sources Validated
- **FACT_Sales** — 3,355 orders, 2023-2025 ✓
- **FACT_Purchases** — purchase orders with delivery tracking ✓
- **FACT_Inventory** — stock movements with quality flags ✓
- **FACT_Budget** — budget vs actual by business line ✓
- **DIM_Products** — 500 products, ABC classified ✓
- **DIM_Customers** — 1,000 customers, RFM segmented ✓

### Data Quality Assessment
| Table | Completeness | Accuracy | Notes |
|-------|-------------|----------|-------|
| FACT_Sales | ✅ High | ✅ High | Simulated dataset |
| FACT_Purchases | ✅ High | ⚠️ Medium | Delivery dates proxy |
| FACT_Inventory | ✅ High | ✅ High | Full movement history |
| FACT_Budget | ✅ High | ✅ High | 3-year coverage |
| FACT_HR | ✅ High | ✅ High | Full payroll data |

### Limitations & Assumptions
- Dataset is simulated for portfolio purposes
- Delivery Delay Days calculated as proxy 
  (Modified Date - Transaction Date)
- Order to Cash Cycle Time based on available date fields
- Inventory Turnover Ratio requires calibration 
  with real operational data

## Process Capability

### Sigma Level Calculation
DPMO = 1,106
Sigma Level = 4 (based on DPMO lookup table)
DPMO Benchmarks:

6 Sigma = 3.4 DPMO    (world class)
5 Sigma = 233 DPMO    (excellent)
4 Sigma = 6,210 DPMO  (good - current level)
3 Sigma = 66,807 DPMO (average industry)

### OEE Breakdown
OEE = Availability × Performance × Quality Rate
OEE = 91% × 95% × 95% = 82%
World Class OEE = 85%
Current Gap = -3pp
Primary constraint: Availability (91% vs 95% target)

## Key Measurement Findings

1. **On-Time Delivery is the most critical gap** — 
   47% vs 85% target represents a 38pp deficit 
   affecting customer satisfaction directly.

2. **Process Cycle Efficiency at 4% indicates systemic waste** — 
   Only 2 hours of value-added time in a 47-hour cycle. 
   22% of process time adds no customer value.

3. **Customer base at tipping point** — 
   268 At Risk customers (41% potential churn) 
   nearly equals 272 Champions. 
   Retention intervention is urgent.

4. **Financial forecasting is strong (97%)** — 
   The problem is execution control, not planning accuracy.

## Deliverables — Measure Phase
- [x] Baseline metrics established
- [x] Data collection plan defined
- [x] Process capability calculated (Sigma, OEE)
- [x] Measurement system validated
- [x] Key gaps quantified
- [x] Control charts for key metrics
- [ ] Detailed VSM with time measurements *(planned)* - partial made 33%
