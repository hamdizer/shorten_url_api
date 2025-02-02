Overview

This project is a simplified version of a URL shortening service, similar to Bit.ly. It allows users to input a long URL and receive a shortened version. When the shortened URL is accessed, it redirects to the original URL.

Features

Backend: RESTful API for URL shortening and redirection.

Frontend: A simple web interface to interact with the API.

Database: Stores long URLs and their corresponding shortened versions.

Validation: Ensures input URLs are valid.

Testing: Unit tests for backend logic and end-to-end tests for API endpoints.

Technologies Used

Backend: Node.js, Express.js, MongoDB

Frontend: HTML, CSS, JavaScript (React/Vue or plain JS)

Testing: Jest, Supertest

Project Structure

url-shortener/
├── backend/
│   ├── server.js        # Express server setup
│   ├── routes.js        # API routes
│   ├── controllers/     # Business logic
│   ├── models/          # Database models
│   └── tests/           # Unit and API tests
├── frontend/
│   ├── index.html       # Web interface
│   ├── styles.css       # Styling
│   ├── app.js           # API communication
├── README.md            # Documentation
├── package.json         # Dependencies and scripts
└── .env                 # Environment variables

Setup Instructions

Prerequisites

Node.js installed

MongoDB database

Installation

Clone the repository:

git clone https://github.com/your-repo/url-shortener.git
cd url-shortener

Install dependencies:

npm install

Set up environment variables in a .env file:

MONGO_URI=your_mongodb_connection_string
BASE_URL=http://localhost:5000

Start the backend server:

npm start

Open frontend/index.html in a browser to use the web interface.

Testing

Run unit and API tests:

npm test

Edge Cases Handled

Invalid URLs

Non-existent shortened URLs

Duplicate URLs

Database failures

Future Enhancements

User authentication for managing URLs

Analytics for tracking URL usage

Custom short URLs

License

MIT License
Response:

{
  "shortenedUrl": "https://yourdomain.com/abc123"
}

2. Redirect to Original URL

Endpoint: GET /{shortened_id}

Description: Redirects to the original URL corresponding to the shortened ID.

Example: Accessing https://yourdomain.com/abc123 redirects to https://example.com.

