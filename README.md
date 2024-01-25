# Quiz Management API

## Description

This project is a web application designed to manage quiz questions and choices. It utilizes FastAPI for creating API endpoints and SQLAlchemy for Object-Relational Mapping (ORM). The application supports operations to create questions and choices, read individual questions and their associated choices, and maintain these entities in a PostgreSQL database.

## Installation Instructions

### Prerequisites

- Python 3.7+
- pip

### Steps

1. **Clone the repository**  
   Clone this repository to your local machine using git or download the source code directly.

2. **Install Dependencies**  
   Navigate to the project directory and install the required dependencies using pip: `pip install -r requirements.txt`

## Setup Environment

1. Create a `.env` file in the project root directory.
2. Add the following environment variable: `URL_DATABASE=postgresql://user:password@localhost/dbname`
3. Replace `user`, `password`, `localhost`, and `dbname` with your PostgreSQL database credentials.

## Usage

To run the application, use the following command: `uvicorn main:app --reload`
The API will be available at `http://127.0.0.1:8000`.

### Endpoints

- `GET /questions/{question_id}`: Fetch a single question by its ID.
- `GET /choices/{question_id}`: Fetch all choices related to a given question ID.
- `POST /questions/`: Create a new question with associated choices.

## Dependencies

- FastAPI
- SQLAlchemy
- psycopg2-binary
- uvicorn
- python-dotenv

Refer to `requirements.txt` for specific version details.






