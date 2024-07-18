# Range-Query Optimization Project

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)

## Introduction
The Range-Query Optimization Project focuses on optimizing range queries in databases to improve performance and efficiency. It leverages advanced algorithms and data structures to handle large datasets and complex query requirements.

## Features
- Efficient range query handling
- Support for multiple data types and structures
- Optimized indexing for fast query processing
- Scalable solution for large datasets

## Technologies Used
- Programming Language: C++
- Database: PostgreSQL, MySQL
- Algorithms: Segment Trees, Interval Trees, B-Trees
- Tools: Docker, SQLAlchemy

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/sanjaikrp/range-query-optimization.git
    ```
2. Navigate to the project directory:
    ```sh
    cd range-query-optimization
    ```
3. Install the dependencies:
    ```sh
    pip install -r requirements.txt
    ```
4. Set up the database and environment variables:
    ```sh
    cp .env.example .env
    ```
5. Run the database migrations:
    ```sh
    python manage.py migrate
    ```
6. Start the development server:
    ```sh
    python manage.py runserver
    ```

## Usage
1. Open your web browser and navigate to `http://localhost:8000`.
2. Use the provided interface or API endpoints to execute range queries and analyze performance.


- `POST /api/index/create` - Create a new index
  - Request Body: 
    ```json
    {
        "type": "B-Tree" | "Segment Tree" | "Interval Tree",
        "columns": ["column1", "column2"]
    }
    ```
  - Response: 
    ```json
    {
        "message": "Index created successfully"
    }
    ```
