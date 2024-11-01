# Playwright Cucumber Testing Framework

Cucumber is a popular behavior-driven development (BDD) tool that allows developers and stakeholders to collaborate on defining and testing application requirements in a human-readable format. 
TypeScript is a powerful superset of JavaScript that adds optional static typing, making it easier to catch errors before runtime. By combining these two tools, we can create more reliable and maintainable tests.

# Overview
This project implements a testing framework using Playwright and Cucumber for automated UI testing of the Udacity catalog. The framework supports search functionality and validates results against a mocked API response.

# Features
1. Automated navigation to the Udacity catalog.
2. Search functionality for specific terms.
3. UI results validation against mocked API responses.
4. Cucumber integration for behavior-driven development (BDD).

# Requirements
Node.js (v14 or higher)
npm (Node Package Manager)
TypeScript
Playwright
Cucumber
Chai (for assertions)
Installation

### Setup:

1. Clone or download the project: git clone <repository-url>
2. Extract and open in the VS-Code
3. `npm install` to install the dependencies
4. `npx playwright install` to install the browsers
5. `npm run test` to execute the tests
6. To run a particular test change  
```
  paths: [
            "src/test/features/featurename.feature"
         ] 
```
7. Use tags to run a specific or collection of specs
```
npm run test --TAGS="@test or @add"
```

### Folder structure
0. `src\pages` -> All the page (UI screen)
1. `src\test\features` -> write your features here
2. `src\test\steps` -> Your step definitions goes here
3. `src\hooks\hooks.ts` -> Browser setup and teardown logic
4. `src\hooks\pageFixture.ts` -> Simple way to share the page objects to steps
5. `src\helper\env` -> Multiple environments are handled
6. `src\helper\types` -> To get environment code suggestions
7. `src\helper\report` -> To generate the report
8. `config/cucumber.js` -> One file to do all the magic
9. `package.json` -> Contains all the dependencies
10. `src\helper\auth` -> Storage state (Auth file)
11. `src\helper\util` -> Read test data from json & logger

