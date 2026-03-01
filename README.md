# API Test Automation Framework (Postman + Newman + CI/CD)
End-to-end API test automation framework built with Postman and executed in a CI/CD pipeline using Newman and GitHub Actions.Focused on validating REST API functionality, response integrity, and system robustness through realistic and repeatable test workflows.

## Test Structure
### Smoke Tests
Core functional workflow validation:
- Resource retrieval and response verification
- Dynamic request chaining using runtime data
- Entity creation and validation
- Data clean-up to ensure repeatable and stable execution
- Status code and response integrity validation

### Negative Tests
Validation of system robustness and error handling:
- Missing or invalid authentication scenarios
- Empty or malformed request payloads
- Invalid data types and structures
- Unexpected fields and edge case handling

## CI/CD Integration
- Automated execution on every push and pull request
- Independent execution of Smoke and Negative test suites
- Secure API key handling via GitHub Secrets
- HTML and JUnit reporting
- Artifact storage for traceability and debugging

## Tech Stack
- Postman
- Newman CLI
- JavaScript (Postman scripting)
- GitHub Actions
- REST API testing

## Project Structure
api-test-framework/
├── postman/
│   ├── api_test_framework.collection.json
│   └── api_test_framework.environment.json
├── .github/workflows/
│   └── postman.yml
└── README.md