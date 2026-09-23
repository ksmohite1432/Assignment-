🎬 Movie Booking – Seat Booking

BCA 1st Semester Project – Feature Set I

A simple academic database-design project for managing movie seat booking. This project demonstrates the complete booking flow from entering customer details to confirming a seat reservation.

---

📌 Project Overview

The Movie Booking – Seat Booking system is designed to manage the basic information required for booking seats for a movie show.

The project covers five main feature areas:

1. Customer Details
2. Movie Details
3. Theatre Details
4. Show Details
5. Seat Booking

The project includes:

- Algorithm
- Flowchart
- ER Diagram
- Database entities and relationships
- Primary Key and Foreign Key identification
- Seat availability checking
- Booking confirmation process

---

🎯 Objective

The main objective of this project is to design a simple and organized Movie Seat Booking System that can:

- Store customer information
- Store movie information
- Manage theatre information
- Manage movie shows
- Display available seats
- Allow seat selection
- Check seat availability
- Confirm seat booking
- Store booking information
- Display booking confirmation

---

🔄 Booking Process

START
   ↓
Enter Customer Details
   ↓
Validate Customer Details
   ↓
Is Customer Information Valid?
   ├── NO → Display "Invalid Details"
   │          ↓
   │      Enter Details Again
   │
   └── YES
        ↓
    Select Movie
        ↓
    Display Movie Details
        ↓
    Select Theatre
        ↓
    Display Theatre Details
        ↓
    Select Show (Date & Time)
        ↓
    Display Available Seats
        ↓
    Select Seat
        ↓
    Is Seat Available?
       ├── NO → Display "Seat Not Available"
       │          ↓
       │      Select Another Seat
       │
       └── YES
            ↓
       Confirm Seat Booking
            ↓
       Store Booking Details
            ↓
       Display Booking Confirmation
            ↓
           END

---

📋 Feature Set I

Feature| Description
Customer Details| Stores customer information
Movie Details| Stores movie information
Theatre Details| Stores theatre information
Show Details| Manages movie show date and time
Seat Booking| Handles seat selection and booking

---

🧮 Algorithm

Step-by-Step Procedure

1. START the movie seat-booking process.
2. Enter customer details such as Customer ID, Name, Phone, and Email.
3. Validate the entered customer information.
4. Check whether the customer information is valid.
5. If the customer information is invalid, display "Invalid Details" and ask the customer to enter the details again.
6. If the customer information is valid, continue with movie selection.
7. Select a movie from the available movie list.
8. Display the selected movie details.
9. Check whether the selected movie is available.
10. If the movie or show is not available, ask the customer to select another available movie or show.
11. If the movie and show are available, select the required theatre.
12. Display the selected theatre details.
13. Select the required show, date, and time.
14. Display the available seats for the selected show.
15. Select the required seat or seats.
16. Check whether the selected seat or seats are available.
17. If the seat is not available, display "Seat Not Available" and ask the customer to select another seat.
18. If the seat is available, confirm the seat booking.
19. Reserve the selected seat or seats.
20. Store the booking details.
21. Display the booking confirmation.
22. END the movie seat-booking process.

---

📊 ER Diagram

The database design consists of the following entities:

1. CUSTOMER

Attribute| Key
Customer_ID| PK
Customer_Name| —
Phone| —
Email| —

2. MOVIE

Attribute| Key
Movie_ID| PK
Movie_Name| —
Genre| —
Language| —
Duration| —

3. THEATRE

Attribute| Key
Theatre_ID| PK
Theatre_Name| —
Location| —
Total_Seats| —

4. SHOW

Attribute| Key
Show_ID| PK
Show_Date| —
Show_Time| —
Movie_ID| FK
Theatre_ID| FK

5. SEAT

Attribute| Key
Seat_ID| PK
Seat_Number| —
Theatre_ID| FK

6. SEAT_BOOKING

Attribute| Key
Booking_ID| PK
Customer_ID| FK
Show_ID| FK
Seat_ID| FK
Booking_Date| —
Booking_Status| —

---

🔗 Database Relationships

The following relationships are used in the ER diagram:

CUSTOMER     1 ────────< N  SEAT_BOOKING

MOVIE        1 ────────< N  SHOW

THEATRE      1 ────────< N  SHOW

THEATRE      1 ────────< N  SEAT

SHOW         1 ────────< N  SEAT_BOOKING

SEAT         1 ────────< N  SEAT_BOOKING

Relationship Explanation

- One Customer can have multiple seat bookings.
- One Movie can have multiple shows.
- One Theatre can have multiple shows.
- One Theatre can contain multiple seats.
- One Show can have multiple seat bookings.
- One Seat can be associated with multiple booking records across different shows.

---

🔑 Keys Used

Primary Key (PK)

A Primary Key uniquely identifies each record in an entity.

Examples:

Customer_ID
Movie_ID
Theatre_ID
Show_ID
Seat_ID
Booking_ID

Foreign Key (FK)

A Foreign Key connects one entity with another entity.

Examples:

Movie_ID       → SHOW
Theatre_ID     → SHOW
Theatre_ID     → SEAT
Customer_ID    → SEAT_BOOKING
Show_ID        → SEAT_BOOKING
Seat_ID        → SEAT_BOOKING

---

📁 Project Structure

A suggested GitHub repository structure is:

Movie-Booking-Seat-Booking/
│
├── README.md
│
├── Algorithm/
│   └── Movie_Booking_Algorithm.pdf
│
├── Flowchart/
│   └── Movie_Booking_Flowchart.png
│
├── ER-Diagram/
│   └── Movie_Booking_ER_Diagram.png
│
├── Documentation/
│   └── Movie_Booking_Documentation.pdf
│
└── Assets/
    └── Images/

«File and folder names can be changed according to the actual files uploaded to the repository.»

---

🛠️ Technologies / Concepts

This academic project focuses mainly on:

- Database Management System (DBMS)
- Entity Relationship Model
- ER Diagrams
- Primary Keys
- Foreign Keys
- Cardinality
- Data Validation
- Seat Availability
- Database Relationships
- Algorithm Design
- Flowchart Design

---

🎓 Academic Information

Project: Movie Booking – Seat Booking
Feature Set: I
Course: BCA – Bachelor of Computer Applications
Semester: 1st Semester
Project Type: Academic Assignment

---

📌 Important Notes

- This project is created for academic and educational purposes.
- The design focuses on the specified Feature Set I.
- The system does not include additional features such as online payment, cancellation, offers, login, or reviews.
- PK and FK relationships are clearly identified in the database design.
- The algorithm and flowchart follow the same logical booking process as the ER diagram.

---

👨‍💻 Author

Karan Mohite

BCA – 1st Semester

---

⭐ Project Summary

The Movie Booking – Seat Booking project demonstrates how a basic movie reservation system can be represented using an algorithm, flowchart, and Entity Relationship Diagram (ER Diagram).

The system follows a simple process:

Customer
   ↓
Movie
   ↓
Theatre
   ↓
Show
   ↓
Available Seats
   ↓
Seat Selection
   ↓
Availability Check
   ↓
Booking Confirmation

---

📚 Educational Purpose

This project is intended to demonstrate fundamental BCA 1st-semester DBMS and system-design concepts through a simple, structured, and easy-to-understand movie seat-booking example.
