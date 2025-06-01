# Matatu Booking System 🚐

A Command-Line Interface (CLI) system for managing matatus, routes, and bookings. Built using Python, SQLAlchemy ORM, and a relational SQLite database. Designed to meet Phase 3 project requirements.

##  Features

- **Matatu Management**
  - List all matatus
  - Create, view, and delete matatus
  - View all routes assigned to a matatu

- **Route Management**
  - List all routes
  - Create, view, and delete routes
  - View all bookings on a route

- **Booking Management**
  - List all bookings
  - Create, view, and delete bookings
  - Book matatus by route

##  Technologies Used

- Python 3
- SQLAlchemy ORM
- SQLite (for local development)
- Pipenv (for dependency management)

##  Project Structure

python-matatu-booking-system/
├── lib/
| ├──database.py
│ ├── cli.py # Entry point CLI interface
│ ├── helpers.py # Logic for CRUD operations
| ├──seed.py
│ └── models/
│ ├── init.py
│ └── model_1.py
├── matatu_booking.db
├── Pipfile # Pipenv dependencies
└── README.md



## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/python-matatu-booking-system.git
cd python-matatu-booking-system
2. Set Up Virtual Environment
pip install pipenv
pipenv install
pipenv shell
3. Initialize the Database
python db/setup.py
4. Run the CLI
python lib/cli.py
  Sample Data
After setting up the database, you can run the CLI to manually input matatus, routes, and bookings.

  Best Practices Followed
Separation of concerns using a models/ directory

SQLAlchemy ORM for DB interaction

Input validation and error handling in CLI

CRUD operations implemented in helper functions

Persistent CLI loop with navigation