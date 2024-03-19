# Revenue-Insights using Power BI

This project aims to analyze hotel booking data to uncover trends that will maximize revenue for the hotel.

Through data cleaning, data modeling in Power BI, and DAX measure development, I analyzed critical hotel performance metrics including:
- RevPAR (Revenue per Available Room)
- ADR (Average Daily Rate)
- Occupation %
- Realization %
- DSRN (Daily Sellable Room Nights)
- DBRN (Daily Booked Room Nights)
- DURN (Daily Utilized Room Nights)

Transformation steps involved:
 - Step 1: Since the weekends are different(Friday and Saturday) in this insudtry we are deleting the column day_type in power query.
 - Step 2: Loaded the data.
 - Step 3: For data modelling, star schema is created and defined relationships between fact table and dimension tables.
 - Step 4: Remove "W" from "week no" column from table dim_date by creating another column from "week no" column using DAX functions.
 - Step 5: Created a table called key_measures and created the following measures.
       Revenue = SUM(fact_bookings[revenue_realized])



- Step 6: filtered out week 32 while creating dashboard since week 32 had only one day.
- Step 7: Created filters(slicers) for city, room_type, month and week.
- Step 8: Created card type for revenue, RevPAR, ADR, Occupancy %, Realization %, DSRN and below every card created arrow icons to show the week-on-week change.
- Step 9: Created a Donut chart to show the oocupancy percentage by category.
- Step 10: Created a Dual axis line chart for ADR, RevPAR and Occupancy % by Month and week no.
- Step 11: Created text table for the key metrics.
- Step 12: Created a line and clustered column chart for Realization % and ADR Vs Booking Platform


![Screenshot 2024-03-19 173514](https://github.com/sowmiya-rajkumar/Revenue-Insights-using-Power-BI/assets/98767488/2226283b-2654-4923-8765-b12b2931f517)

