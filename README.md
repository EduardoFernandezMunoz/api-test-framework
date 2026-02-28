# API Test Automation Framework (Postman + Newman + CI/CD)
End-to-end API test automation framework built with Postman and executed in a CI/CD pipeline using Newman and GitHub Actions.
Focused on validating REST API functionality, response integrity, and system robustness through realistic and repeatable test workflows.

## Test flow
The collection covers a complete scenario:
* **GET requests** – data retrieval and response validation.
* **POST creation** – dynamic data and request chaining.
* **DELETE cleanup** – ensures repeatability and stable test execution.
* **Negative testing** – validation of error handling, status codes, and edge cases.

## Key Practices
* REST API testing
* Dynamic data and request chaining
* Response and status code validation
* Structured negative testing
* Environment and secret management
* CI/CD integration for continuous quality feedback

## CI/CD
* Automated execution on every push and pull request with:
* Newman CLI
* Secure API key handling
* HTML and JUnit test reports
* Artifact storage for traceability

## Project Structure
api-test-framework/
├── postman/
│   ├── api_test_framework.collection.json
│   └── api_test_framework.environment.json
├── .github/workflows/
│   └── api-tests.yml
└── README.md