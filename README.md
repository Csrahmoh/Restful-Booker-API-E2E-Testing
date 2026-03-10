Restful-Booker API End-to-End Testing Project
This project demonstrates a robust End-to-End (E2E) API Testing suite for the Restful-Booker platform. It focuses on validating the full lifecycle of booking management through automated scripts, environment variables, and precise technical documentation.

Project Overview
The objective of this suite is to ensure the reliability and security of the Restful-Booker API by testing core functionalities:

Secure Authentication: Dynamic token generation and handling for authorized access to protected endpoints.

Full CRUD Operations: Creating, retrieving, updating (Full/Partial), and deleting bookings to ensure data consistency.

Data Integrity: Rigorous validation of HTTP status codes, response structures (Schema), and business logic.

Tools & Technologies
Postman: For request organization, collection management, and environment configuration.

JavaScript: For writing custom test scripts and automated assertions (PM API).

Environments: Utilizing variables for Base URL and Dynamic Tokens to ensure script reusability.

GitHub: For version control and professional project documentation.

Project Architecture
Collections/: Includes the Postman Collection organized into dedicated folders: Auth, Booking, and HealthCheck.

Environments/: Environment variables for seamless switching between different test setups.

Scripts/: Embedded JavaScript tests for automated verification of response data and performance.

Test Scenarios & Logic
1. Authentication (Auth)
POST /auth: Generates a secret token. Tests ensure a valid token is returned only for correct credentials (admin/password123).

2. Booking Lifecycle (CRUD)
POST /booking: Creates a new booking entry. Validates successful bookingid generation.

GET /booking: Tests retrieval by ID and advanced filtering using Query Parameters (First Name, Last Name, and Dates).

PUT /booking: Full update operation requiring Cookie-based Token Authorization.

PATCH /booking: Partial updates to verify the ability to modify specific fields without affecting the entire resource.

DELETE /booking: Ensures permanent removal of bookings and verifies the system prevents access to deleted IDs.

3. System Reliability
GET /ping: A health check endpoint to confirm API availability and server uptime.

How to Run & Verify
Import: Drag the Collection and Environment JSON files into your Postman workspace.

Setup: Select the Restful-Booker Environment from the environment dropdown.

Execute:

Use the Collection Runner to execute the entire test suite.

Review the Test Results tab for green indicators confirming all assertions passed.

Developed by
Rahaf Almohammadi

LinkedIn: www.linkedin.com/in/rahaf-almohammadi-

Project Link: Restful-Booker API Testing Workspace
