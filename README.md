# inn-hotels-bookings
# Hotel Booking Cancellation Prediction

## Project Overview
INN Hotels Group, a chain of hotels in Portugal, faces a significant issue with booking cancellations. These cancellations not only impact revenue but also increase operational costs, especially with last-minute cancellations. The rise of online booking channels has changed customer behavior, making it more difficult for hotels to predict cancellations. This project aims to develop a machine learning model to predict the likelihood of a booking being canceled, enabling the hotels to formulate effective cancellation policies and mitigate losses.

## Objective
The goal of this project is to:
1. Analyze the factors that influence hotel booking cancellations.
2. Build a predictive model to identify bookings that are likely to be canceled.
3. Provide insights to help formulate more profitable cancellation and refund policies.

## Data Description
The dataset contains various attributes of customers' booking details. Below is the data dictionary:

| Column Name                | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| `Booking_ID`                | Unique identifier of each booking                                           |
| `no_of_adults`              | Number of adults                                                           |
| `no_of_children`            | Number of children                                                         |
| `no_of_weekend_nights`      | Number of weekend nights booked/stayed (Saturday or Sunday)                 |
| `no_of_week_nights`         | Number of weeknights booked/stayed (Monday to Friday)                       |
| `type_of_meal_plan`         | Meal plan selected by the customer:                                         |
|                            | - Not Selected: No meal plan selected                                       |
|                            | - Meal Plan 1: Breakfast                                                    |
|                            | - Meal Plan 2: Half board (breakfast + one meal)                            |
|                            | - Meal Plan 3: Full board (breakfast, lunch, and dinner)                    |
| `required_car_parking_space`| Customer requested car parking space (0 - No, 1 - Yes)                      |
| `room_type_reserved`        | Room type reserved (encoded by the hotel group)                             |
| `lead_time`                 | Number of days between booking date and arrival date                        |
| `arrival_year`              | Year of arrival                                                            |
| `arrival_month`             | Month of arrival                                                           |
| `arrival_date`              | Day of the month for arrival                                                |
| `market_segment_type`       | Market segment of the booking                                               |
| `repeated_guest`            | Repeated guest flag (0 - No, 1 - Yes)                                       |
| `no_of_previous_cancellations` | Number of previous cancellations by the customer                        |
| `no_of_previous_bookings_not_canceled` | Number of previous bookings not canceled by the customer        |
| `avg_price_per_room`        | Average price per day of the reservation (in euros)                         |
| `no_of_special_requests`    | Total number of special requests made by the customer                       |
| `booking_status`            | Booking status flag (1 - Canceled, 0 - Not Canceled)                        |

## Exploratory Data Analysis (EDA) Questions
1. **What are the busiest months in the hotel?**
   - Analyze which months see the highest volume of bookings to understand seasonality trends.

2. **Which market segment do most guests come from?**
   - Examine the market segment breakdown to understand the distribution of guests.

3. **What are the differences in room prices across market segments?**
   - Analyze how room prices vary by market segment, considering dynamic pricing strategies.

4. **What percentage of bookings are canceled?**
   - Calculate the overall cancellation rate to assess the extent of the issue.

5. **What percentage of repeating guests cancel?**
   - Understand how cancellation behavior differs between first-time and repeating guests.

6. **Do special requests affect booking cancellations?**
   - Investigate whether guests with special requests have a higher likelihood of cancellation.
