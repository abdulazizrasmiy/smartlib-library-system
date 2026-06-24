# System Architecture

## SmartLib System Architecture

SmartLib is designed as a modular web-based library automation system.

## Main Components

### 1. User Interface

The user interface allows students, teachers, librarians, and administrators to interact with the system.

Main pages:

- Login page
- Book catalog
- Book detail page
- Reservation page
- User profile
- Admin dashboard
- Statistics page

### 2. Backend

The backend handles business logic, database operations, authentication, book reservations, borrowing processes, and reporting.

Backend responsibilities:

- User authentication
- Book management
- Reservation management
- Borrowing and return control
- Overdue tracking
- Report generation

### 3. Database

The database stores information about books, users, reservations, borrowing history, returns, and statistics.

Main tables:

- Users
- Books
- Book Copies
- Reservations
- Borrowing Records
- Faculties
- Reports

### 4. API Layer

The API layer allows different parts of the system to communicate with each other. It can also be used for future mobile application integration.

### 5. Admin Panel

The admin panel is used by librarians and system administrators to manage the library data.

## General Workflow

1. User searches for a book.
2. System checks book availability.
3. User creates a reservation.
4. Librarian confirms and issues the book.
5. System records borrowing date and return date.
6. User returns the book.
7. System updates the book status.
8. Statistics are generated automatically.

## Security Principles

- Secret keys are not stored in the repository.
- Real user data is not included.
- Database files are not uploaded.
- Environment variables are stored separately.
