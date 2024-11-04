# Postman Usage Guide

## Introduction
Postman is a powerful tool for testing APIs, enabling you to create, share, document, and test APIs easily. This guide provides an overview of how to use Postman effectively.

## Installation
1. Download Postman from the [official website](https://www.postman.com/downloads/).
2. Install it on your system following the installation instructions.

## Key Features
- **Collections**: Group related requests for better organization.
- **Environments**: Manage variables across different settings (development, testing, production).
- **Testing**: Write tests using JavaScript to validate responses.
- **Mock Servers**: Simulate API responses to test applications without a live backend.
- **Documentation**: Automatically generate API documentation for your collections.

## Creating a Request
1. Open Postman and click on **New**.
2. Select **Request**.
3. Name your request and add it to a collection if desired.
4. Choose the request type (GET, POST, etc.) and enter the URL.
5. Add parameters, headers, and body as needed.
6. Click **Send** to execute the request.

## Using Variables
- **Global Variables**: Variables accessible across all collections and requests.
- **Environment Variables**: Variables specific to a selected environment.

### How to Create Variables
1. Go to the **Manage Environments** (gear icon in the top right).
2. Click on **Add** to create a new environment or select an existing one.
3. Add key-value pairs for your variables.

### Exporting Variables
To export global or environment variables:
1. Go to the **Manage Environments**.
2. Click on the **...** icon and select **Export**.
3. Save the JSON file to your desired location.

## Testing APIs
Postman allows you to write tests using JavaScript. To add tests:
1. Go to the **Tests** tab of your request.
2. Write your test code, for example:
   ```javascript
   pm.test("Status code is 200", function () {
       pm.response.to.have.status(200);
   });
   ```
3. Click **Send** to run the request and view test results.

## Documentation
Postman can automatically generate documentation for your collections:
1. Click on the collection name.
2. Go to the **Documentation** tab.
3. Fill in the details and publish your documentation.

## Conclusion
Postman is an essential tool for API development and testing. With features for organization, testing, and documentation, it streamlines the API workflow.

For more information, visit the [Postman Learning Center](https://learning.postman.com/docs/getting-started/introduction/).
