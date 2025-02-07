Hotel Revenue Analytics Dashboard

Overview
This interactive Power BI dashboard provides actionable insights into hotel revenue performance by tracking 26+ hospitality KPIs, including Occupancy %, ADR, RevPAR, and Cancellation Trends. Designed for hotel managers and revenue teams, it enables data-driven decisions to optimize pricing, reduce revenue leakage, and improve operational efficiency.

Key Metrics & KPIs
Core Metrics

Revenue Realized: Total revenue from bookings.

Occupancy %: Ratio of successful bookings to total room capacity.

ADR (Average Daily Rate): Revenue per booked room.

RevPAR (Revenue Per Available Room): Revenue per available room (occupied or not).

Cancellation % and No-Show Rate: Track booking attrition drivers.

Realization %: Successful check-outs as a percentage of total bookings.

Operational Metrics

DBRN (Daily Booked Room Nights): Average daily bookings.

DSRN (Daily Sellable Room Nights): Average daily room capacity.

DURN (Daily Utilized Room Nights): Average daily check-outs.

Trend Analysis

Week-over-Week (WoW) Changes: Revenue, Occupancy, ADR, and RevPAR trends.

Technical Implementation
Data Model
Star Schema: Built with fact_bookings, fact_aggregated_bookings, dim_date, and dim_rooms.

Relationships: Established between fact and dimension tables for seamless filtering.


Dashboard Features
Interactive Visualizations:

Time-series charts for Revenue, Occupancy, and ADR trends.

Heatmaps for peak booking periods and room-class demand.

Donut charts for cancellation/no-show breakdowns.

Time Intelligence:

Week-over-Week (WoW) and Month-over-Month (MoM) trend filters.

Drill-Downs:

Analyze data by date, hotel property, or room class.

Insights & Business Impact
Revenue Leakage Identification:

15% revenue loss attributed to no-shows and last-minute cancellations.

Recommended pre-payment policies for high-risk bookings.

Pricing Strategy Optimization:

20% higher ADR for Premium rooms during weekends vs. weekdays.

Dynamic pricing suggestions for underperforming room classes.

Operational Efficiency:

12% increase in DURN by reallocating staff during high-occupancy periods.

Technical Challenges & Solutions
Data Granularity:

Aggregated daily bookings (fact_aggregated_bookings) with capacity data while maintaining granularity in fact_bookings for cancellation analysis.

Dynamic Week-over-Week Calculations:

Used FILTER(ALL(dim_date)) to isolate previous week’s data without breaking context.

Performance Optimization:

Reduced load times by 30% using summarized tables for frequently accessed metrics.

