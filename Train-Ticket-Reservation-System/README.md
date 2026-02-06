# Train Ticket Reservation System

A comprehensive web-based application for managing train ticket reservations. This system allows users to search for trains, book tickets, and manage their reservations, while administrators can manage trains, schedules, and fares.

## Features

### User Features
- **User Registration & Login**: Secure user authentication and account management
- **Train Search**: Search trains between stations with various filters
- **Ticket Booking**: Book tickets with real-time fare calculation
- **Booking History**: View and track past bookings and reservations
- **User Profile Management**: Update personal information and change password
- **Fare Enquiry**: Check fare details between stations
- **Payment Integration**: Secure payment processing for bookings

### Admin Features
- **Train Management**: Add, update, and cancel trains
- **Schedule Management**: Update train schedules and availability
- **Fare Management**: Set and manage ticket fares
- **Admin Dashboard**: Monitor system activity and bookings

## Technology Stack

- **Backend**: Java, Servlets
- **Frontend**: HTML5, CSS
- **Build Tool**: Maven (pom.xml)
- **Database**: MySQL (with JDBC)

## Project Structure

```
Train-Ticket-Reservation-System/
├── src/
│   ├── application.properties          # Configuration file
│   └── com/jaya/
│       ├── beans/                      # Data models and exceptions
│       ├── constant/                   # Constant values (response codes, user roles)
│       ├── service/                    # Business logic interfaces
│       ├── servlets/                   # HTTP request handlers
│       └── utility/                    # Database and utility classes
├── WebContent/
│   ├── *.html                          # User interface pages
│   ├── *.css                           # Stylesheets
│   └── WEB-INF/                        # Web application configuration
├── pom.xml                             # Maven project configuration
└── Dummy-Database.md                   # Sample database documentation
```

## Key Components

### Beans (Models)
- `UserBean`: User information and authentication
- `AdminBean`: Admin user details
- `TrainBean`: Train information
- `BookingDetails`: Reservation details
- `HistoryBean`: Booking history

### Services
- `UserService`: User authentication and profile management
- `TrainService`: Train search and information
- `BookingService`: Ticket booking operations

### Servlets
- **User Operations**: Registration, login, profile management, booking
- **Train Operations**: Search, view, and booking
- **Admin Operations**: Train management and scheduling
- **Payment**: Payment processing

### Utilities
- `DBUtil`: Database connection and operations
- `TrainUtil`: Train-related utility functions

## Setup Instructions

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- Apache Tomcat 9 or higher
- MySQL database
- Maven

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/jayasri-stack/online_tickect_management_system.git
   cd online_tickect_management_system/Train-Ticket-Reservation-System
   ```

2. **Configure Database**
   - Create a MySQL database
   - Update `application.properties` with database credentials
   - Import the database schema (see Dummy-Database.md)

3. **Build the Project**
   ```bash
   mvn clean install
   ```

4. **Deploy to Tomcat**
   - Copy the generated WAR file to Tomcat's `webapps` directory
   - Start Tomcat server

5. **Access the Application**
   - Open browser and navigate to `http://localhost:8080/Train-Ticket-Reservation-System`

## Usage

### User Workflow
1. Register a new account
2. Login with credentials
3. Search for available trains
4. Book tickets and proceed to payment
5. View booking history
6. Manage profile and preferences

### Admin Workflow
1. Login to admin panel
2. Manage trains (add, update, cancel)
3. Update schedules and availability
4. View and manage all bookings

## Configuration

Edit `application.properties` to configure:
- Database connection details
- Server properties
- Application settings

## License

This project is licensed under the MIT License.

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

## Support

For issues, questions, or suggestions, please contact the development team or open an issue in the repository.
