# OrangeHRM API Testing – Manual QA Portfolio

## Project Overview

This project is a hands-on API testing portfolio using the OrangeHRM demo application. The purpose is to practice API testing, validate endpoint behavior, verify authentication, perform negative testing, and document test results using Postman.

This project was developed through self-directed learning and practical testing exercises.

## Tools & Technologies

- **Postman** – API testing and request validation
- **Postman Documenter** – API documentation
- **Microsoft Excel / Google Sheets** – Test planning, test cases, and bug reporting
- **Git & GitHub** – Version control and project documentation
- **OrangeHRM Demo** – Application under test

## Scope of Testing

The project covers the following areas:

### 1. Authentication
- OAuth 2.0 authentication
- Verify authenticated requests
- Unauthorized access testing
- Invalid access token testing
- Refresh token testing

### 2. Employee Management
- Get Employee List
- Create Employee
- Delete Employee

### 3. Admin Modules
- Get Admin Modules
- Verify access with and without authentication

### 4. Employee Contact Details
- Update Employee Contact Details
- Get Employee Contact Details

### 5. Negative Testing
- Empty request body
- Missing required fields
- Delete nonexistent employee
- Invalid access token
- Unauthorized requests

## Test Documentation

| Document | Description |
|---|---|
| Test Plan | Testing objectives, scope, and approach |
| Test Cases | Test scenarios, steps, and expected results |
| Bug Report Summary | Summary of observed issues and findings |
| Test Evidence | Screenshots of API testing results |

## API Documentation

The API documentation is published using Postman Documenter.

**[View OrangeHRM API Documentation](https://documenter.getpostman.com/view/59587715/2sBYHaPx22)**

## Test Results

Testing includes positive and negative scenarios with HTTP status code validation, response body verification, authentication checks, and response time assertions.

Observed responses include:

- `200 OK` – Successful requests
- `401 Unauthorized` – Authentication required or invalid
- `422 Unprocessable Entity` – Request validation failure
- `404 Not Found` – Requested record not found

These status codes represent observed test scenarios, not necessarily application defects.

## Learning Outcomes

Through this project, I practiced:

- Understanding REST API fundamentals
- Working with HTTP methods and status codes
- Implementing OAuth 2.0 authentication in Postman
- Writing and executing API test cases
- Performing positive and negative testing
- Validating JSON responses
- Documenting test results and potential defects
- Organizing QA deliverables using GitHub

## Application Under Test

**OrangeHRM Demo:** https://opensource-demo.orangehrmlive.com/

## Disclaimer

This project is intended for educational and portfolio purposes. Testing was performed against the publicly available OrangeHRM demo environment. Test results may vary depending on the demo application's availability and data state.