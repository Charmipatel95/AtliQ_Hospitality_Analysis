## :hotel:	AtliQ's Hospitality Analysis

 I have worked on this analysis project.

:link: Link to the [Challenge](https://codebasics.io/challenge/codebasics-resume-project-challenge)

:link: Link to [Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiOWFlYWEwZDctN2NhYi00ZmUzLTg4ZmYtZWNiMDIwY2I3NmY1IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

:link: Link to LinkedIn post 

## :memo: Problem statement

Atliq Grands owns multiple five-star hotels across India. They have been in the hospitality industry for the past 20 years. Due to strategic moves from other competitors and ineffective decision-making in management, Atliq Grands are losing its market share and revenue in the luxury/business hotels category. As a strategic move, the managing director of Atliq Grands wanted to incorporate “Business and Data Intelligence” in order to regain their market share and revenue. However, they do not have an in-house data analytics team to provide them with these insights.

Their revenue management team had decided to hire a 3rd party service provider to provide them insights from their historical data.


### :scroll: Task List

You are a data analyst who has been provided with sample data and a mock-up dashboard to work on the following task. You can download all relevant documents from the download section.

- Create the metrics according to the metric list. 
- Create a dashboard according to the mock-up provided by stakeholders. 
- Create relevant insights that are not provided in the metric list/mock-up dashboard.

### :open_file_folder: Dataset Understanding

In simpler terms, here's what data we have available for analysis:
Data set is mainly divided into two types of table namely:
- **Dimension Tables**: These contain static information about customers and products
- **Fact Tables**: These contain transactional data.

 Let's understand the dataset: 
 
- :date: **dim_date:**
    - date: Dates in May, June, and July.
    - mmm yy: Date in the format of mmm yy (month year).
    - week no: Unique week number for each date.
    - day_type: Indicates if the day is a Weekend or Weekday.

- :hotel: **dim_hotels:**
    - **7** distinct hotels
    - **2** categories:
       - Business
       - Luxury
   - **4** cities:
     - Bangalore
     -  Delhi
     -  Mumbai
     -  Hyderabad

- 🚪🛏️ **dim_rooms:**
    - **7** distinct hotels
    - **2** categories:
      - Business
      - Luxury
    - room_id: Type of rooms
      - RT1
      - RT2
      - RT3
      - RT4
    - room_class: **4** Types of Room
      - Standard
      - Elite
      - Premium
      - Presidential

- 📋 **fact_aggregated_bookings:**
    - property_id:  Unique ID for each hotel
    - check_in_date: Customer check-in dates
    - room_category: Type of room
    - successful_bookings: Successful room bookings for a specific date.
    - capacity: Maximum room count available on a specific date.

- 📝 **fact_bookings:**
    - booking_id: Unique Booking ID for each customer. 
    - property_id: Unique ID for each hotel.
    - booking_date: Date the customer booked their room.
    - check_in_date: Customer check-in date.
    - check_out_date: Customer checkout date.
    - no_guests: Number of guests in the room.
    - room_category: Type of room. 
    - booking_platform: Booking method
    - ratings_given: Customer ratings for hotel services.
    - booking_status: Booking status (Cancelled, Checked Out, No Show).
    - revenue_generated: Amount generated from the booking.
    - revenue_realized: Final revenue based on booking status (deductions for cancellations).

## :bar_chart: Provided Mock-up Dashboard
![mock up dashboard_atliq grands](https://github.com/Charmipatel95/AtliQ_Hospitality_Analysis/assets/154671418/ca0f2bca-9a1e-446c-9f7d-0b459423bde6)


## :chart_with_upwards_trend:	Data Model
![hospitality- data model](https://github.com/Charmipatel95/AtliQ_Hospitality_Analysis/assets/154671418/86499013-3273-45eb-9550-5ca3d5e80446)

## 📶Overall Analysis View

https://github.com/Charmipatel95/AtliQ_Hospitality_Analysis/assets/154671418/d4174be0-9102-4a26-88c6-763a3c670254

## :chart_with_downwards_trend: Home Page
![homepage 1](https://github.com/Charmipatel95/AtliQ_Hospitality_Analysis/assets/154671418/1f53ca08-6b21-4bfe-9cd6-7cdad6f74e04)

![hp 2](https://github.com/Charmipatel95/AtliQ_Hospitality_Analysis/assets/154671418/3207b755-840a-4912-89d5-ca827997bf9d)

## :chart_with_downwards_trend:	 More Insights

![MI 1](https://github.com/Charmipatel95/AtliQ_Hospitality_Analysis/assets/154671418/5880933b-bf86-416e-a4c4-f01a8981fcf3)

![mi 2](https://github.com/Charmipatel95/AtliQ_Hospitality_Analysis/assets/154671418/cee4342b-9094-4967-96e8-41766f16c35e)

## :mortar_board:	Learning from this Project 
- It seems like many hotels have a common cancellation policy where guests can cancel their booking without any charge as long as it's done before three months prior to the booking date. However, if the cancellation happens after that timeframe, guests might incur a fee ranging from 60 to 90% of the total booking cost.
- I've become adept at utilizing bookmarks and selections to fulfill diverse needs. One notable application is how I've streamlined page navigation within the dashboard, leveraging these tools to enhance efficiency.
- I have learned that in hotel industry follow three types of pricing Flat pricing, Weekday / Weekend pricing , Dynamic pricing. It is advisable that business should adapt Weekday / Weekend pricing or Dynamic pricing in order to increase the business.

## ✍🏻 Some Important insights from the Dashboard

Here are some key insights gleaned from the Dashboard:

- Mumbai emerges as the top revenue generator, raking in 669 million, closely trailed by Bangalore, Hyderabad, and Delhi.
- AtliQ Exotica stands out among the seven property types, boasting impressive figures: 320 million in revenue, a rating of 3.62, occupancy at 57.3%, and a 24.4% cancellation rate.
- AtliQ Blu boasts the highest occupancy rate at 62%.
- Week 24 stands as the peak revenue-generating period, clocking in at 139.58 million.
- Delhi leads the pack in both occupancy and rating, followed by Hyderabad, Mumbai, and Bangalore.
- Elite room types witness the highest number of bookings but also experience a notable cancellation rate.
- A clear correlation emerges between Rating and Occupancy, indicating a strong positive relationship. Hotels with lower ratings tend to have lower occupancy rates.
- Similarly, a significant negative correlation is evident between Rating and Cancellation Rate. Hotels with lower ratings often experience higher cancellation rates.

