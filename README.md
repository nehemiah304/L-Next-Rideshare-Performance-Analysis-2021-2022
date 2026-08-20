# L-Next-Rideshare-Performance-Analysis-2021-2022

<img width="1439" height="808" alt="L-Next Rideshare Performance Analysis_ 2021–2022" src="https://github.com/user-attachments/assets/c23f2a96-eedb-412b-9525-ce1dca4288c1" />

## 🔍 Overview
This project presents an interactive dashboard tracking L-Next Rideshare's performance from 2021–2022, covering revenue, riders, profit margin, and cost trends across time, rider type, and season to surface where the business is growing and where profitability is under pressure.

### Tools Used: 
Power BI (assumed based on layout/styling — flag if this was actually built on another platform, since the nav bar and "Add new widgets" option aren't standard Power BI conventions).

## 🎯 Objectives

- Track total revenue, COGS, rider count, and profit margin trends year-over-year
- Understand how revenue and ridership have grown from 2021 into 2022
- Identify which days of the week and hours generate the most profit/revenue
- Compare revenue contribution from registered vs. casual riders
- Understand seasonal revenue patterns to guide planning

## ❓ Business Questions

- How have total revenue, COGS, rider count, and profit margin changed vs. last year?
- How have revenue and ridership trended monthly from Jan 2021 to Oct 2022?
- Which days of the week generate the highest average profit?
- What are the peak revenue hours for each day of the week?
- What share of revenue comes from registered riders vs. casual riders?
- How does revenue vary by season?

## 📚 Dataset Description
Source: Rideshare/bike-share transactional dataset (hourly ride records, 2021–2022).
Scope: ~1M rider records, $6M total revenue.
Data Type: Hourly ride-level operational data.
Key Fields: Date, Hour, Day of Week, Season, Rider Type (Registered/Casual), Revenue, COGS.

## 🛠 Tools & Technologies Used

- Power BI (KPI cards, slicers, DAX-driven YoY comparisons)
- Power Query (data cleaning & transformation)
- Interactive Year filter
- KPI cards, area/line trend chart, heat-map matrix (day-of-week and hourly), donut chart, bar chart

## 🧹 Data Cleaning and Preparation

- Removed duplicate ride records
- Handled missing values across revenue, rider type, and time fields
- Corrected data types (dates, hours, currency)
- Standardized day-of-week and season labels
- Verified date/hour fields for accurate trend and heat-map aggregation
- Checked for anomalies in revenue and rider count values

## 📈 Key Trends Discovered
- Explosive year-over-year growth across the board. Total revenue hit $6M (+208.5% vs. last year), rider count reached 1M (+166.7%), and COGS rose to $19K (+126.5%) — revenue grew faster than costs, though profit margin still dipped slightly to 0.69 (-0.12% vs. last year).

- A sharp step-change in early 2022. The Revenue vs. Riders trend is relatively flat and modest through all of 2021, then jumps sharply around January 2022 and sustains a much higher, steadier level through October 2022 — pointing to a specific expansion event (new market, pricing change, or product launch) rather than gradual organic growth.

- Profit is fairly evenly spread across the week, with Thursday leading. Thursday ($313 avg) and Monday ($308) post the highest average daily profit, while Sunday ($282) is lowest — the spread between best and worst day is narrow, suggesting demand isn't concentrated in a few "power days."

- Clear commute-driven hourly peaks on weekdays. The hourly revenue table shows strong morning (8–9am) and especially evening (5–6pm) spikes on weekdays — Thursday at 5pm ($1,244) and Wednesday at 6pm ($1,178) stand out — while Friday and Saturday evenings (7–9pm) also run high, reflecting leisure/nightlife demand layered on top of commuting.

- Registered riders dominate revenue. Registered riders generate 81.4% of revenue versus just 18.6% from casual riders — the business is heavily subscription/membership-driven rather than one-off usage.

- Revenue varies meaningfully by season. Season 3 leads with $1.83M, followed by Season 2 ($1.70M) and Season 4 ($1.60M), while Season 1 trails well behind at just $0.86M — a more than 2x gap between the strongest and weakest season.

## 📈 Trends and Behavioral Patterns
The dashboard shows a business that scaled dramatically in a short window — the early-2022 step-change suggests something structural changed (expansion, marketing push, or pricing shift) rather than steady organic growth, and it's worth digging into what drove it so it can be replicated. Demand is commuter-shaped (weekday morning/evening peaks) but layered with weekend leisure activity, and revenue is heavily concentrated in registered riders, meaning retention matters more than one-off acquisition. The weakest season generating less than half of the top season's revenue is the clearest opportunity area — either a genuine seasonal demand issue or a sign the service isn't yet reaching riders effectively during that period.

## 📊 Dashboard Development (Project Requirements)

- KPI row: Total Revenue, COGS, No. of Riders, Profit Margin, each with YoY comparison, plus a Year filter
- Revenue vs. Riders Trend (dual-metric area/line chart, Jan 2021–Oct 2022)
- Average Profit by Day of Week (heat-map matrix)
- Hourly Revenue by Weekday (heat-map table)
- Percentage Revenue by Rider Type (donut chart: registered vs. casual)
- Revenue by Season (bar chart)

## 💡 Recommendations

- Investigate what drove the early-2022 step-change in revenue and riders, and evaluate whether it can be replicated in other markets or periods
- Build targeted campaigns to boost Season 1 revenue, which lags more than 2x behind the top season
- Double down on registered-rider retention (loyalty perks, subscription tiers) given they drive over 80% of revenue
- Optimize driver/vehicle availability around weekday morning and evening peaks, plus Friday/Saturday evenings
- Monitor the slight YoY dip in profit margin closely — costs may need tighter control even as revenue scales
- Explore casual-to-registered conversion strategies to grow the smaller but potentially high-upside casual segment

## Conclusion:
This project demonstrates the ability to build an interactive dashboard connecting time-based, rider-type, and seasonal data to revenue and profitability outcomes. Beyond answering the six core business questions, the analysis surfaces a clear pattern: growth has been explosive but concentrated around a single early-2022 inflection point, and the business's revenue base is heavily reliant on registered riders and specific seasons — making growth-driver analysis and seasonal balancing the two highest-value next steps.
