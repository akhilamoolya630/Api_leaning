# Api_leaning
Here is an updated version including your understanding about URLs and API endpoints:
API Basics

What is an API?
API (Application Programming Interface) acts as a bridge between the frontend and backend.

It allows the frontend and backend to communicate.

APIs define endpoints (URLs) where requests are sent and responses are received.

API Endpoint vs Page URL
Page URL
Used to display web pages to users.
Visible in the browser address bar.


Examples:
/login
/dashboard
/profile

Example:
Plain text
https://collegeportal.com/login
API Endpoint
Used by the frontend to communicate with the backend.
Usually contains /api (common convention).
Not necessarily visible to users.
Examples:
Plain text
https://collegeportal.com/api/login
https://collegeportal.com/api/students

Difference
Page URL
API Endpoint
Displays pages
Transfers data
Used by users
Used by applications

Example: /dashboard
Example: /api/students

Login Flow
User enters username and password.
User clicks Login.

Frontend sends a POST request to the API endpoint /api/login.

Backend verifies credentials.
Backend returns a response.

Frontend redirects the user.
Browser URL changes from /login to /dashboard.

HTTP Methods
GET
Retrieves/view data.
Does not modify data.

Example: Viewing a student dashboard.

POST
Creates/stores new data.
Example: Creating a student account.

PUT
Updates existing data.
Example: Updating a student's password.

DELETE
Deletes existing data.
Example: Removing a student's record.

How Data Travels
User enters data in the frontend.
Frontend sends the data through an HTTP request.

Data is usually sent in JSON format inside the request body.

Backend receives and processes the data.
Example:
JSON
{
  "username": "Akshatha",
  "password": "1234"
}

Flow:
Plain text
Frontend → HTTP Request → Internet → Backend → Database

HTTP Request Structure
Plain text
HTTP Request
├── URL (API Endpoint)
├── Method (GET/POST/PUT/DELETE)
├── Headers
└── Body (User Data)

Important Point
HTTP requests carry the data.
HTTP does not permanently store data.
The database stores data permanently.

HTTP vs HTTPS
HTTP
HyperText Transfer Protocol.
Data is transferred in plain text.
Less secure.

Example:
Plain text
http://example.com

HTTPS
HyperText Transfer Protocol Secure.
Encrypts data using SSL/TLS.
More secure.

Example:
Plain text
https://example.com

Which One Should We Use?
✅ HTTPS should always be used in modern applications because it protects passwords and sensitive data.

Quick Interview Summary
API acts as a bridge between the frontend and backend. API endpoints are specific URLs used for communication. Page URLs display pages to users, while API endpoints transfer data. HTTP requests carry data between the frontend and backend, and HTTPS is the secure version of HTTP used in modern applications.
