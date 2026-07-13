# BookStore API Testing with Postman

## Overview

This project demonstrates API testing using Postman for a BookStore REST API. It covers the complete book lifecycle by creating a new book, retrieving its details, and deleting it. The collection uses JavaScript to generate dynamic test data and validate API responses automatically.

## Tools & Technologies

- Postman
- REST API
- JavaScript
- JSON
- Postman Collection Variables

## API Endpoints Tested

- **POST** - Add Book
- **GET** - Retrieve Book by ID
- **DELETE** - Delete Book

## Features

- Dynamic generation of test data using Postman's built-in random variables.
- Automatic creation of unique:
  - Book Name
  - ISBN
  - Aisle
  - Author Name
- Collection variables are used to share data between requests.
- Automated response validation using JavaScript test scripts.
- Status code verification.
- Response body validation.
- End-to-end API workflow testing.

## Test Flow

1. Generate random book information.
2. Send a POST request to create a new book.
3. Save the generated Book ID.
4. Retrieve the book using a GET request.
5. Validate the returned book information.
6. Delete the created book using a DELETE request.
7. Verify that the book was deleted successfully.

## Validations Performed

### POST Request
- Status Code = 200
- Success message validation
- Save generated Book ID

### GET Request
- Status Code = 200
- Verify returned book contains:
  - book_name
  - isbn
  - aisle
  - author

### DELETE Request
- Status Code = 200
- Verify successful deletion message

## Project Structure

```
BookStore-API-Testing/
│
├── BookStoreTesting.postman_collection.json
├── README.md
└── screenshots/
```

## How to Run

1. Import the Postman collection.
2. Open the collection in Postman.
3. Run the collection using the Collection Runner.
4. Review the execution results and test assertions.

## Skills Demonstrated

- API Testing
- REST API Validation
- JavaScript in Postman
- Dynamic Test Data Generation
- Collection Variables
- Automated Assertions
- End-to-End API Testing
