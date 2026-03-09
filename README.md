# Restful-Booker API End-to-End Testing Project 

This project demonstrates a comprehensive **End-to-End (E2E) API Testing** suite for the **Restful-Booker** application. It covers the entire lifecycle of booking management, from authentication to CRUD operations, ensuring data integrity and system reliability.

## Project Overview
The goal of this project is to validate the core functionalities of the [Restful-Booker API](https://restful-booker.herokuapp.com/), including:
* **Authentication:** Generating tokens for secure access.
* **Booking Management:** Creating, retrieving, updating, and deleting bookings.
* **Data Validation:** Ensuring correct status codes, response structures (Schema), and business logic.

## Tools & Technologies
* **Postman:** For creating and organizing API requests.
* **JavaScript:** For writing dynamic test scripts within Postman.
* **Newman (Optional):** For running collections via Command Line.
* **GitHub:** For version control and documentation.

## Project Structure
* `collections/`: Contains the Postman Collection JSON file with all requests and test scripts.
* `environments/`: Contains the Environment variables (Base URL, Tokens, etc.).
* `reports/`: (Optional) If you run tests via Newman, save your HTML reports here.

## Test Scenarios Covered
1.  **Auth:** Post CreateToken - Validating successful login and token generation.
2.  **Create Booking:** Verifying that a new booking is correctly stored and returns the expected data.
3.  **Get Booking:** Testing retrieval by ID and filtering by name/date.
4.  **Update Booking:** Full (PUT) and Partial (PATCH) updates to ensure data can be modified.
5.  **Delete Booking:** Ensuring a booking is removed and no longer accessible.
6.  **Schema Validation:** Checking that the JSON response matches the expected data types.

## How to Run the Project
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/Restful-Booker-API-E2E-Testing.git](https://github.com/YOUR_USERNAME/Restful-Booker-API-E2E-Testing.git)
    ```
2.  **Import to Postman:**
    * Open Postman.
    * Click **Import** and select the JSON files from the `collections/` and `environments/` folders.
3.  **Run Tests:**
    * Select the imported environment.
    * Open the **Collection Runner**.
    * Click **Run Restful-Booker Suite**.

---
**Contact:** Rahaf Almohammadi. - www.linkedin.com/in/rahaf-almohammadi-.
