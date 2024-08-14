## Python Virtual Environment Setup:

        python3.12 -m venv venv
        source venv/bin/activate # For Linux/macOS
        venv\Scripts\activate # For Windows


## Dependencies Install:
    pip install --upgrade pip
    pip install fastapi uvicorn sqlalchemy alembic pydantic psycopg2-binary
    pip install pytest coverage  # For testing


## Freezing Dependencies:
    pip freeze > requirements.txt


<!-- Project Working Directories -->

.
├── app
│ ├── **init**.py
│ ├── main.py # Entry point of the app (e.g., FastAPI instance)
│ ├── models.py # SQLAlchemy models
│ ├── schemas.py # Pydantic models
│ ├── crud.py # Database operations
│ ├── database.py # Database connection and setup
│ ├── routers # All your routes (endpoints)
│ │ ├── **init**.py
│ │ └── user.py # User-related routes
│ │ └── task.py # Task-related routes
│ ├── utils.py # Utility functions
│ ├── tests # Unit and integration tests
│ │ ├── **init**.py
│ │ └── test_main.py
│ └── alembic # For database migrations
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md # Project documentation
