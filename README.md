Restful-Booker API End-to-End Testing Project
This project demonstrates a robust End-to-End (E2E) API Testing suite for the Restful-Booker platform, focusing on validating the full lifecycle of booking management through automated scripts and precise documentation.

Project Overview
The objective of this suite is to ensure the reliability and security of the Restful-Booker API by testing core functionalities:

Secure Authentication: Dynamic token generation and handling for authorized access.

Full CRUD Operations: Creating, retrieving, updating (Full/Partial), and deleting bookings.

Data Integrity: Rigorous validation of status codes, response structures (Schema), and business logic.

Tools & Technologies
Postman: Request organization and environment management.

JavaScript: Custom test scripts and automated assertions (PM API).

Environments: Using variables for Base URL and Dynamic Tokens to ensure reusability.

GitHub: Version control and technical documentation.

Project Architecture
Collections/: Includes the Postman Collection with organized folders for (Auth, Booking, HealthCheck).

Environments/: Environment variables for seamless switching between test setups.

Scripts/: Embedded JavaScript tests for automated verification of responses.

Test Scenarios & Logic
Authentication (Auth):

POST /auth: Generates a secret token. Tests ensure a valid token is returned for correct credentials.

Booking Lifecycle (CRUD):

POST /booking: Creates a new entry. Validates the bookingid generation.

GET /booking: Retrieval by ID and advanced filtering using Query Parameters (Name, Dates).

PUT /booking: Full update requiring Cookie-based Token Authorization.

PATCH /booking: Partial updates to verify flexibility in data modification.

DELETE /booking: Permanent removal and verification of 404/Deleted status.

System Reliability:

GET /ping: Health check to confirm API availability (201 Created).

How to Run & Verify
Import: Drag the Collection and Environment JSON files into Postman.

Setup: Select the Restful-Booker Environment.

Execute:

Use the Collection Runner to run the entire suite.

Check the Test Results tab for green "PASSED" indicators.

Developed by
Rahaf Almohammadi

🔗 LinkedIn: www.linkedin.com/in/rahaf-almohammadi-

📧 Contact: For collaboration or QA-related inquiries.
