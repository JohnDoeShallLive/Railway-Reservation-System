Railway Reservation System

This project is a Railway Reservation System built using Streamlit and SQLite. It provides functionalities for managing train reservations, including adding trains, booking tickets, viewing available seats, and canceling bookings.

Features

Admin Functions:

Add Train: Add new train details including train number, name, departure date, and destinations.

View Trains: View all trains available in the database.

Search Train:

Search by train number.

Search by starting and ending destinations.

Delete Train: Remove train details and associated seat information.

Passenger Functions:

Book Ticket:

Enter passenger details (name, age, gender).

Select seat type (Window, Aisle, or Middle).

Automatically allocate the next available seat based on preferences.

Cancel Ticket: Cancel a booking by specifying the train number and seat number.

View Seats: Display the seat map of a specific train with booking statuses and passenger details.

Installation and Setup

Prerequisites:

Python 3.7 or above

SQLite installed (optional, as Python includes SQLite by default)

Steps:

Clone the repository:

git clone https://github.com/JohnDoeShallLive/Railway-Reservation-System.git
cd Railway-Reservation-System

Create a virtual environment (optional but recommended):

python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

Install the required packages:

pip install -r requirements.txt

Run the application:

streamlit run main.py

Open the local URL provided by Streamlit (e.g., http://localhost:8501) in your web browser.

Database Structure

The application uses an SQLite database (railway_system.db) with the following tables:

users: Stores user credentials.

username: Text

password: Text

employees: Stores employee credentials and designations.

employee_id: Text

password: Text

designation: Text

trains: Stores train details.

train_number: Text

train_name: Text

departure_date: Text

starting_destination: Text

ending_destination: Text

seats_<train_number>: Dynamic tables for seat allocation per train.

seat_number: Integer (Primary Key)

seat_type: Text

booked: Integer (0 for available, 1 for booked)

passenger_name: Text

passenger_age: Integer

passenger_gender: Text

Usage

Adding a Train:

Navigate to "Add Train" in the sidebar.

Fill in the form with the train details and submit.

Booking Tickets:

Select "Book Ticket" from the sidebar.

Enter train number, seat preferences, and passenger details.

Submit to book the ticket.

Viewing and Canceling Seats:

Use "View Seats" to check the current booking status.

Use "Cancel Ticket" to remove a booking by specifying the train and seat number.

Technologies Used

Frontend: Streamlit

Database: SQLite

Language: Python

Future Enhancements

Integration with payment gateways for ticket purchases.

User authentication for passengers and employees.

Enhanced train scheduling and real-time seat availability updates.

Contributing

Contributions are welcome! To contribute:

Fork the repository.

Create a new branch for your feature (git checkout -b feature-name).

Commit your changes and push them to your fork.

Submit a pull request describing your changes.

Contact - Shreyash Sule

For any queries or suggestions, please contact shreyashsule22@gmail.com
