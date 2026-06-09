# Define Phase

## Problem Statement
The organization faces critical operational gaps affecting 
customer satisfaction, profitability, and process efficiency:

- **On-Time Delivery: 47%** vs industry target of 85%
- **Process Cycle Efficiency: 4%** — 96% of cycle time is waste
- **268 At Risk customers** nearly equal 272 Champions
- **Budget overspend: 11%** despite 97% forecast accuracy

## Voice of Customer (VOC)
| Customer Need | Current Performance | Gap |
|---------------|-------------------|-----|
| On-time delivery | 47% | Critical |
| Product quality | 94% First Pass Yield | Near target |
| Order fulfillment | 3% Stockout Rate | Acceptable |
| Consistent pricing | 11% budget variance | Needs improvement |

## SIPOC Map

| Suppliers | Inputs | Process | Outputs | Customers |
|-----------|--------|---------|---------|-----------|
| 200+ Suppliers | Purchase Orders | Order to Cash | Delivered Products | B2B, Government, Retail |
| Internal Teams | Customer Orders | Purchase to Pay | Invoices | End Customers |
| Warehouses | Inventory Data | Inventory Management | Stock Reports | Internal Teams |

## Project Boundaries
**Start point:** Customer places order  
**End point:** Customer receives product and payment is collected  
**Process in focus:** Order to Cash cycle (701 days average cycle time)

## Key Stakeholders
| Stakeholder | Interest | Impact |
|-------------|----------|--------|
| Executive Leadership | Revenue & profitability | High |
| Supply Chain Team | Delivery performance | High |
| Finance Team | Budget control | Medium |
| Customers | On-time delivery | High |

## CTQ Tree (Critical to Quality)
Voice of Customer (Retailer)
│
├── "I want on-time deliveries"
│       └── CTQ: On-Time Delivery Rate ≥ 85%
│               ├── Driver: Supplier Performance Index ≥ 85
│               ├── Driver: Delivery Delay Days ≤ 3
│               └── Driver: Stockout Rate ≤ 2%
│
├── "I want defect-free products"
│       └── CTQ: First Pass Yield ≥ 95%
│               ├── Driver: DPMO ≤ 233 (5 Sigma target)
│               ├── Driver: Defects Per Unit ≤ 3%
│               └── Driver: OEE ≥ 85%
│
├── "I want to retain my customers"
│       └── CTQ: Customer Retention Rate ≥ 75%
│               ├── Driver: Churn Rate ≤ 25%
│               ├── Driver: At Risk Customers ≤ 10% of base
│               └── Driver: Champions Segment ≥ 40%
│
└── "I want costs under control"
        └── CTQ: Budget Variance ≤ 5%
                ├── Driver: Forecast Accuracy ≥ 95%
                ├── Driver: OPEX within budget ±5%
                └── Driver: Cost per Purchase Line ↓ YoY

## Business Impact
| Area | Current Loss | Opportunity |
|------|-------------|-------------|
| Revenue at risk | 41% delayed orders | +38pp delivery improvement |
| Customer churn | 41% Churn Rate | Retention program for 268 At Risk |
| Process waste | 96% non-value-added time | Cycle time reduction |
| Budget control | 11% overspend | Execution gate reviews |

## Problem Prioritization (Pareto)
Based on business impact, the top 3 priorities are:

1. **On-Time Delivery (47%)** — highest customer impact
2. **Customer Retention (41% Churn)** — direct revenue risk  
3. **Process Cycle Efficiency (4%)** — largest waste opportunity

## Deliverables — Define Phase
- [x] Project Charter
- [x] SIPOC Map
- [x] CTQ Tree
- [x] Stakeholder Analysis
- [x] Problem prioritization
- [ ] VSM — Order to Cash *(in progress)*
- [ ] VSM — Purchase to Pay *(planned)*
- [ ] VSM — Inventory Management *(planned)*
