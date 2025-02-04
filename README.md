# Number Classification API

## Overview
The **Number Classification API** is a RESTful API that analyzes a given number and returns its mathematical properties, including whether it is prime, perfect, Armstrong, and odd/even. It also provides a fun fact about the number using the Numbers API.

## Features
- Classifies numbers as prime, perfect, Armstrong, odd, or even.
- Calculates the sum of the digits.
- Retrieves a fun fact about the number.
- Supports cross-origin resource sharing (CORS).
- Returns responses in JSON format.

## Live API URL
🚀 **Base URL:**
```
https://number-classifyapi.vercel.app/
```

🔹 **Example Endpoint:**
```
https://number-classifyapi.vercel.app/api/classify-number?number=880
```

## API Endpoints

### 1️⃣ Classify a Number
#### **Endpoint:**
```
GET /api/classify-number?number={number}
```
#### **Query Parameters:**
| Parameter | Type  | Description |
|-----------|-------|-------------|
| number    | int   | The number to classify |

#### **Example Request:**
```
GET /api/classify-number?number=880
```
#### **Success Response (200 OK):**
```json
{
    "number": 880,
    "is_prime": false,
    "is_perfect": false,
    "properties": [
        "even"
    ],
    "digit_sum": 16,
    "fun_fact": "880 is the number of 4×4 magic squares."
}
```
#### **Error Response (400 Bad Request):**
```json
{
    "number": "hello",
    "error": true
}
```

## Installation & Setup

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/yourusername/number-classifyapi.git
cd number-classifyapi
```

### 2️⃣ Install Dependencies
```sh
npm install
```

### 3️⃣ Run the API Locally
```sh
npm start
```
The API will be available at:
```
http://localhost:5000
```

## Deployment
The API is deployed using **Vercel**.
To deploy manually:
```sh
vercel --prod
```

## Technologies Used
- **Node.js** - Server-side runtime
- **Express.js** - Web framework for Node.js
- **Axios** - HTTP client for fetching fun facts
- **CORS** - Handling cross-origin requests

## Additional Links
Hire Node.js Developers: https://hng.tech/hire/nodejs-developers

