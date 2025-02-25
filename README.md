# Hotel Booking Prediction

Contributors:
- Kevin Rio Harristyando
- Sekar Saraswati Wibowo
- Theresia Diah Kusumaningrum

## Project Overview 
The hotel industry faces significant challenges related to booking cancellations, which can impact revenue, operational efficiency, and overall customer satisfaction. Key stakeholders include:

- **Hotel Management:** Seeks to minimize revenue loss due to last-minute cancellations.
- **Revenue Management Teams:** Need accurate cancellation predictions to implement dynamic pricing and optimize room allocation.
- **Marketing Departments:** Can target customers more effectively by understanding cancellation patterns.
- **Business Strategy Teams:** Focus on evaluating campaign effectiveness, measuring ROI, and developing actionable strategies for growth.

### Data Understanding
- **Source:** [Hotel Booking Demand Dataset on Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand/data)
- **Description:**  
  This dataset contains 119,389 historical booking records from hotels, which include various features such as booking details, customer demographics, and booking statuses. Each row in the dataset represents a single booking record.

- **Target Variable:**  
  For our classification task, the target variable is **`is_canceled`**, where:
  - `1` indicates that the booking was canceled.
  - `0` indicates that the booking was not canceled.
  - 

### Modelling

We compared the results of 6 different classification algorithms and applied 2 undersampling methods to find the best model.
**Models**
- Logistic Regression
- KNN (K-Nearest Neighbors)
- Decision Tree
- Random Forest
- LightGBM (Light Gradient Boosting Machine)
- XGBoost (Extreme Gradient Boosting)

**Undersampling Methods**
- Random Undersampling
- SMOTE

### Result

## Tableau Dashboard
You can explore our Tableau dashboard [here.](https://public.tableau.com/app/profile/gamma.team/viz/HotelBooking_17403871991650/CancelAnalysis)

## Streamlit Application


### Feature Overview

Below is a table summarizing the key features in the dataset:

| **Feature**                         | **Description**                                                                                               |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| **adr**                             | Average Daily Rate per room (in hotel currency).                                                          |
| **adults**                          | Number of adults in the booking.                                                                          |
| **agent**                           | Travel agent ID handling the booking (can be null).                                                       |
| **arrival_date_day_of_month**       | Day of the month when the arrival is scheduled.                                                           |
| **arrival_date_month**              | Month of arrival (e.g., "January", "February").                                                           |
| **arrival_date_week_number**        | Week number of the arrival date.                                                                          |
| **arrival_date_year**               | Year of arrival.                                                                                          |
| **assigned_room_type**              | Code of the room type actually assigned.                                                                 |
| **babies**                          | Number of babies in the booking.                                                                          |
| **booking_changes**                 | Number of changes made to the booking.                                                                    |
| **children**                        | Number of children in the booking (can be null).                                                          |
| **company**                         | Company ID associated with the booking (can be null).                                                     |
| **country**                         | Country of origin of the customer (can be null).                                                          |
| **customer_type**                   | Type of customer ("Transient", "Contract", "Group", "Transient-Party").                                  |
| **days_in_waiting_list**            | Number of days the booking was on the waiting list before confirmation.                                   |
| **deposit_type**                    | Type of deposit required ("No Deposit", "Non Refundable", "Refundable").                                  |
| **distribution_channel**            | Booking distribution channel (e.g., "TA/TO", "Direct").                                                  |
| **hotel**                           | Type of hotel ("Resort Hotel" or "City Hotel").                                                            |
| **is_canceled**                     | Booking cancellation status (1 = canceled, 0 = not canceled).                                             |
| **is_repeated_guest**               | Indicates if the guest has stayed at the hotel before (1 = Yes, 0 = No).                                  |
| **lead_time**                       | Number of days between booking and arrival.                                                               |
| **market_segment**                  | Market segment category (e.g., "Direct", "Corporate", "Online TA").                                       |
| **meal**                            | Type of meal plan booked (e.g., "BB" for Bed & Breakfast).                                                |
| **previous_bookings_not_canceled**  | Number of previous bookings that were not canceled.                                                       |
| **previous_cancellations**          | Number of previous bookings that were canceled.                                                           |
| **required_car_parking_spaces**     | Number of car parking spaces requested by the customer.                                                  |
| **reserved_room_type**              | Code of the room type initially reserved.                                                                 |
| **reservation_status**              | Final reservation status ("Canceled", "Check-Out", "No-Show").                                            |
| **reservation_status_date**         | Date when the reservation status was last updated.                                                       |
| **stays_in_week_nights**            | Number of weekday nights (Monday-Friday) included in the booking.                                         |
| **stays_in_weekend_nights**         | Number of weekend nights (Saturday/Sunday) included in the booking.                                       |
| **total_of_special_requests**       | Total number of special requests made (e.g., extra bed, high floor).                                      |
                                        
