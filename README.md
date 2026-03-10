# Restful-Booker API End-to-End Testing Project

---

## Project Overview
This project demonstrates a robust **End-to-End (E2E) API Testing** suite for the **Restful-Booker** platform. It focuses on validating the full lifecycle of booking management through automated scripts, environment variables, and precise technical documentation.

The objective of this suite is to ensure the reliability and security of the [Restful-Booker API](https://restful-booker.herokuapp.com/) by testing core functionalities:

* **Secure Authentication**: Dynamic token generation and handling for authorized access to protected endpoints.
* **Full CRUD Operations**: Creating, retrieving, updating (Full/Partial), and deleting bookings to ensure data consistency.
* **Data Integrity**: Rigorous validation of HTTP status codes, response structures (Schema), and business logic.

---

## Tools & Technologies
* **Postman**: For request organization, collection management, and environment configuration.
* **JavaScript**: For writing custom test scripts and automated assertions (PM API).
* **Environments**: Utilizing variables for Base URL and Dynamic Tokens to ensure script reusability.
* **GitHub**: For version control and professional project documentation.

---

## Test Scenarios & Logic

### 1. Authentication (Auth)
**POST /auth**: Generates a secret token. Tests ensure a valid token is returned only for correct credentials (admin/password123).

### 2. Booking Lifecycle (CRUD)
* **POST /booking**: Creates a new booking entry. Validates successful `bookingid` generation.
* **GET /booking**: Tests retrieval by ID and advanced filtering using **Query Parameters** (First Name, Last Name, and Dates).
* **PUT /booking**: Full update operation requiring **Cookie-based Token Authorization**.
* **PATCH /booking**: Partial updates to verify the ability to modify specific fields without affecting the entire resource.
* **DELETE /booking**: Ensures permanent removal of bookings and verifies the system prevents access to deleted IDs.

### 3. System Reliability
**GET /ping**: A health check endpoint to confirm API availability and server uptime.

---

## How to Run & Verify
1. **Import**: Drag the Collection and Environment JSON files into your Postman workspace.
2. **Setup**: Select the `Restful-Booker Environment` from the environment dropdown.
3. **Execute**: Use the **Collection Runner** to execute the entire test suite and review the **Test Results** tab.

---

## Contact
**Rahaf Almohammadi**
* **LinkedIn**: [www.linkedin.com/in/rahaf-almohammadi-](https://www.linkedin.com/in/rahaf-almohammadi-)
* **Postman Workspace**: [View Project](https://rahaf1102000-4299454.postman.co/workspace/Rahaf-Almohammadi's-Workspace~dcef00ea-921b-4ad7-8d90-77d0194678f2/collection/53022018-28a540b9-cacf-4b63-8fc6-41609b69908f)
