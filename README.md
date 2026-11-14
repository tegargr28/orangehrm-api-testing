# OrangeHRM API Testing Portfolio

A hands-on Manual QA project focused on API testing using Postman and the OrangeHRM demo application.

This project demonstrates my understanding of API testing fundamentals, authentication, positive and negative test scenarios, response validation, and test documentation.

## Project Overview

The purpose of this project is to test REST API functionality in OrangeHRM, identify unexpected responses, validate API behavior, and document test results.

**Application Under Test:** [OrangeHRM Demo](https://opensource-demo.orangehrmlive.com/)

## Project Highlights

| Deliverable | Description | Link |
|---|---|---|
| API Documentation | Postman collection and request examples | [View Documentation](https://documenter.getpostman.com/view/59587715/2sBYHaPx22) |
| Test Plan | Testing objectives, scope, and approach | [View Test Plan](https://docs.google.com/document/d/147TBN5hBC9CunrU-qOGl794brlgYrfcI-6yqHHWDEgk/edit?usp=drive_link) |
| Test Cases | Positive and negative test scenarios | [View Test Cases](https://docs.google.com/spreadsheets/d/1_yGFSrc6b3wdXQ5epDyxw6GOHOBG7LrgBFvy6ITcSfo/edit?usp=drive_link) |
| Bug Report Summary | Summary of documented testing findings | [View Excel Report](documentation/OrangeHRM_Bug_Report_Summary.xlsx) |
| Test Evidence | Screenshots of API execution results | [View Test Evidence](test-evidence/) |

## Testing Scope

The project covers the following API testing areas:

- **Authentication:** OAuth 2.0 Authorization Code with PKCE, access token validation, refresh token, and unauthorized access.
- **Employee Management:** Retrieve employee list, create employee, and delete employee.
- **Employee Contact Details:** Retrieve and update employee contact information.
- **Admin Modules:** Validate authenticated and unauthenticated access.
- **Negative Testing:** Invalid access token, missing or empty request body, invalid employee ID, and unauthorized requests.
- **Response Validation:** HTTP status codes and API response structures.

## Testing Results

The following HTTP responses were observed during testing:

| Scenario | Observed Status Code |
|---|---:|
| Retrieve Employee List | 200 OK |
| Create Employee | 200 OK |
| Delete Employee | 200 OK |
| Retrieve Contact Details | 200 OK |
| Update Contact Details | 200 OK |
| Access Admin Modules Without Authentication | 401 Unauthorized |
| Access Admin Modules With Authentication | 200 OK |
| Create Employee With Empty Request Body | 422 Unprocessable Content |
| Create Employee Without Last Name | 422 Unprocessable Content |
| Delete Non-existent Employee | 404 Not Found |

*Note: These are observed results from the tested scenarios, not a claim that every API endpoint has been tested.*

## Tools & Technologies

- **Postman** — API requests, authentication, response validation, and documentation.
- **OrangeHRM Demo** — Application Under Test.
- **Google Docs & Google Sheets** — Test Plan and Test Case documentation.
- **Microsoft Excel** — Bug Report Summary.
- **Git & GitHub** — Version control and project repository.

## Project Structure

```text
orangehrm-api-testing/
├── documentation/
│   └── OrangeHRM_Bug_Report_Summary.xlsx
├── postman/
│   └── OrangeHRM API Testing.postman_collection.json
├── test-documentation/
│   ├── Test Case OrangeHRM
│   └── Test Plan OrangeHRM
├── test-evidence/
│   ├── authentication/
│   ├── contact-details/
│   └── employee-management/
├── .gitignore
└── README.md
```

## Key Learning Outcomes

Through this self-directed project, I gained practical experience in:

- Understanding REST API fundamentals and HTTP methods.
- Working with OAuth 2.0 authentication.
- Creating and executing API test scenarios using Postman.
- Performing positive and negative testing.
- Validating HTTP status codes and response bodies.
- Preparing test documentation and bug report summaries.
- Organizing test evidence and managing projects using GitHub.

## About Me

I am an Informatics Engineering graduate currently developing my skills in Quality Assurance through self-directed learning and hands-on practice.

I am interested in pursuing a career as a Junior QA Engineer, with a focus on Manual Testing and API Testing.

