# Global Airbnb Performance Dashboard

A Power BI dashboard analyzing Airbnb listing and review data across major global cities — covering growth trends, market share, pricing, ratings, review behavior, and host trust signals.

---

## Dashboard Preview

### Page 1 — New Listings Over Time
![Page 1](assets/page1_growth.png)

### Page 2 — Market Share & Ratings
![Page 2](assets/page2_market_ratings.png)

### Page 3 — Review Frequency, Seasonality & Trust
![Page 3](assets/page3_reviews_trust.png)

---

## Project Summary

| Metric | Value |
|---|---|
| Total Listings | 279,712 |
| Cities | 10 |
| Total Hosts | 182,024 |
| Property Types | 144 |
| Total Reviews | 5,373K |

---

## Dashboard Pages

### Page 1 — New Listings Over Time

Tracks Airbnb's listing growth from 2008 to 2021 across six lifecycle phases: Introduction, Growth, Maturity, Decline, Reinvention, and COVID-19. Broken down by room type: Entire place, Private room, Shared room, Hotel room.

**Key Insights:**
- 2015 was the peak year for new listings
- 2016–2017 saw a slowdown due to tightening local regulations
- Airbnb became profitable in H2 2016; 2017 was its first full profitable year
- Growth resumed from 2018 before COVID-19 caused a sharp decline
- Hotel room listings increased notably from 2018 onward

---

### Page 2 — Market Share & Ratings

**Market Share — Pareto Chart**
Superhost vs non-Superhost listings by city with cumulative % line.

**Key Insights:**
- Paris, NYC, and Sydney account for nearly half of total listings and 59% of total reviews
- Paris leads in both listings and reviews — hotel rooms there cost roughly twice the price of an Airbnb listing

**Avg Price by Room Type:**

| Room Type | Avg Price |
|---|---|
| Hotel room | $800 |
| Entire place | $673 |
| Shared room | $580 |
| Private room | $462 |

**Ratings — Bookmark Toggle**

Uses a Power BI bookmark to switch between two views triggered by clicking the icons in the "Select the detail level" panel:
- **Overall Rating** (star icon) — Bar chart of average rating per city
- **Detailed Rating** (magnifying glass icon) — Table with per-city scores across Accuracy, Cleanliness, Communication, Location, and Value

| City | Accuracy | Cleanliness | Communication | Location | Value |
|---|---|---|---|---|---|
| Bangkok | 9.5 | 9.4 | 9.6 | 9.2 | 9.3 |
| Cape Town | 9.6 | 9.5 | 9.7 | 9.7 | 9.5 |
| Hong Kong | 9.2 | 9.0 | 9.4 | 9.6 | 9.0 |
| Istanbul | 9.3 | 9.1 | 9.5 | 9.4 | 9.2 |
| Mexico City | 9.7 | 9.6 | 9.8 | 9.8 | 9.6 |
| New York | 9.6 | 9.3 | 9.7 | 9.6 | 9.4 |
| Paris | 9.6 | 9.2 | 9.7 | 9.7 | 9.3 |
| Rio de Janeiro | 9.6 | 9.4 | 9.8 | 9.8 | 9.3 |
| Rome | 9.6 | 9.5 | 9.7 | 9.6 | 9.4 |
| Sydney | 9.5 | 9.2 | 9.7 | 9.7 | 9.3 |

**Key Insights:**
- Mexico City and Rio de Janeiro are the highest-rated cities overall
- Hong Kong (89.7) and Istanbul (91.1) are the lowest-rated
- Cleanliness and Value consistently score the lowest across all cities

---

### Page 3 — Review Frequency, Seasonality & Trust

**Review Frequency — Pareto Chart**

**Key Insights:**
- 86.5% of reviewers wrote only once
- 98.8% of reviewers wrote 3 times or fewer
- One outlier wrote 283 reviews — last two on 13-Oct-2020 for two Bangkok listings (data error or globe-trotter?)

**Seasonality — 100% Stacked Area Chart**
Monthly review share across Paris, Rome, New York, Mexico City, and Sydney.

**Key Insights:**
- Paris and Rome dominate review share from April to August, reflecting peak European summer travel
- New York spikes in November and December during the holiday season

**Trust — Host Verification Matrix**

| | No Profile Pic | Profile Pic |
|---|---|---|
| Identity Not Verified | 0.3% | 32.6% |
| Identity Verified | 0.1% | 66.9% |

**Key Insight:** Over two-thirds of hosts are fully identity-verified with a profile picture. Unverified and anonymous profiles are minimal.

---

## Files

```
├── Air_BnB_Performance_dashboard.pbix          # Power BI report file
├── Global-Airbnb-Performance-Dashboard.pptx    # Presentation deck
├── Air_BnB_Performance_dashboard.pdf           # PDF export of all pages
├── assets/
│   ├── air_bnb_logo.png
│   ├── Color_Palette.png
│   ├── Dotted_Line_rectangle.png
│   ├── Magnifying_glass.png
│   ├── SHIELD.png
│   └── Star.webp
└── README.md
```

---

## Tools Used

- **Power BI Desktop** — Data modeling, DAX measures, report design
- **Power Query** — Data transformation and shaping
- **Bookmarks** — Toggle between Overall and Detailed rating views

---

## How to Open

1. Download `Air_BnB_Performance_dashboard.pbix`
2. Open in Power BI Desktop
3. If prompted, update the data source path to your local data files

---

## Author

**Gagan B P** · [databygagan.com](https://databygagan.com) · [GitHub](https://github.com/GaganBP)
