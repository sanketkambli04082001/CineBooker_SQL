
# CineBooker



## Description

CineBooker is an innovative Movie Management System (MMS), designed to enhance the movie-going experience. This comprehensive case study introduces a carefully designed approach to movie management, using basic techniques and tools,leveraging the power of relational database management systems (RDBMS). It efficiently tracks movie data, user preferences, and theater information, providing a seamless platform for both movie enthusiasts and theater operators.This system offers accurate tracking of movie screenings,timings, user bookings and theater capacities, and also shows available seats for the next user ensuring optimal resource utilization. It simplifies billing processes by using various payment methods,maintains customer records, and analyzes movie ratings, Helping theaters provide great movie experiences while making operations smoother.
## Features

- Users can easily browse movie listings, check showtimes, and book tickets with just a few clicks, enhancing convenience and saving time.
- Theater owners can gain valuable insights into customer preferences and booking trends.
- CineBooker supports various payment methods, ensuring a seamless and secure transaction process for users.
- By efficiently managing seat bookings and optimizing theater capacities, cinema owners can maximize revenue potential and ensure an enjoyable movie experience for customers.


## Database Structure

- UserTable:
    - u_id(PK)
    - u_name
    - u_email
    - u_contact
- MovieTable:
    - mov_id(Primary Key)
    - mov_name
    - genre
    - duration_hours
    - release_date
    - rating
- Theater-info Table:
    - t_id (PK)
    - t_name
    - location
    - cast_datetime
    - capacity
    - movie_id (FK-Movie_Table)
- Booking Information Table (Booking):
    - b_id(PK)
    - book_seat
    - user_id (FK-User_Table)
    - theater_id (FK-Theater_info_Table)
- Payment Table:
    - p_id(PK)
    - b_id(FK-Booking_Table)
    - amount
    - Payment_method

## ER-Diagram

![App Screenshot](https://github.com/sanketkambli04082001/CineBooker_SQL/assets/99606067/49160331-b866-4949-a5d2-c9190d8b5c54)
