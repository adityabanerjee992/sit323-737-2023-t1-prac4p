# Simple Calculator API

This is a simple REST API for performing basic arithmetic operations. The API supports addition, subtraction, multiplication and division.

## Prerequisites

To run this API, you must have Node.js installed on your machine.

## Installation

1. Clone this repository to your local machine.
2. Install dependencies by running the following command in your terminal:

```
npm install

```

3. Start the server with the following command:

```
node index.js

```

4. The server should now be running at `http://localhost:3040`.

## API Endpoints

### Addition

Performs addition of two numbers.

**Request:**

```
GET /add?n1=4&n2=5

```

**Response:**

```
{
  "statuscode": 200,
  "data": 9
}

```

### Subtraction

Performs subtraction of two numbers.

**Request:**

```
GET /subtract?n1=10&n2=6

```

**Response:**

```
{
  "statuscode": 200,
  "data": 4
}

```

### Multiplication

Performs multiplication of two numbers.

**Request:**

```
GET /multiply?n1=3&n2=5

```

**Response:**

```
{
  "statuscode": 200,
  "data": 15
}

```

### Division

Performs division of two numbers.

**Request:**

```
GET /divide?n1=10&n2=2

```

**Response:**

```
{
  "statuscode": 200,
  "data": 5
}

```

## Error Handling

If an error occurs during the processing of a request, the API returns an error response with an appropriate HTTP status code and an error message in JSON format.

## Logging

The API logs all requests and errors using the Winston logging library. The logs are written to two files: `error.log` and `combined.log`. If the API is not running in production mode, the logs are also printed to the console.
