# QA Automation Project

## Project Overview
This project demonstrates UI automation testing using Playwright and API testing using Postman on the SauceDemo and JSONPlaceholder practice websites.

## Tools & Technologies
- Playwright
- JavaScript
- Node.js
- Postman
- GitHub Actions
- Chromium

## 1. UI Automation Testing

**Website:** https://www.saucedemo.com/

Automated test scenarios include:
- Login with valid and invalid credentials
- Products display
- Add and remove products from cart
- Checkout process
- Form validation
- Product sorting
- Product details
- Continue shopping

**Execution Results:**
- Total test cases: 14
- Passed: 14
- Failed: 0
- Browser: Chromium

### Run UI Tests

Install dependencies:

```bash
npm ci
```

Install Chromium:

```bash
npx playwright install chromium
```

Run tests:

```bash
npx playwright test --project=chromium
```

## 2. API Testing

**API:** https://jsonplaceholder.typicode.com

Postman collection includes six requests:
1. GET - Get All Posts
2. GET - Get Single Post
3. GET - Filter Posts by User
4. POST - Create New Post
5. PUT - Update Existing Post
6. DELETE - Delete Post

The collection includes 23 test assertions covering response status codes, response data, and expected values.

**Note:** JSONPlaceholder is a testing API. POST, PUT, and DELETE operations are simulated and do not permanently modify the server data.

The Postman collection is available in:

`postman/QA_API_Testing_Collection.json`

## 3. Test Documentation

The project includes:
- `Test_Cases.xlsx` — Manual test cases and execution results.
- Bug report workbook — Bug Reports and Test Execution Summary sheets.

No confirmed defects were identified in the tested scenarios.

## 4. CI/CD

GitHub Actions is configured to run Playwright tests automatically when code is pushed or a pull request is created for the main or master branch.

## Project Scope

This project demonstrates practical experience with UI automation, API testing, test documentation, and basic CI/CD workflows.