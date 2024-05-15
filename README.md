# Cypress Technical Assessment

## Installation clone the project repositry

```bash
  git clone respositry Url
```
## Install Dependencience
```bash
npm Install
```
## Run the cypress Test 
```bash
npx cypress run
npx cypress open
```
## Allure reporting configuration
Link - https://github.com/Shelex/cypress-allure-plugin

Download the allure plugin "npm i -D @shelex/cypress-allure-plugin"

Update cypress config ts file by adding these codes
  - import allureWriter from "@shelex/cypress-allure-plugin/writer";
  - allureWriter(on, config);

Update tsconfig json file by adding @shelex
  - "types": ["cypress", "node", "@shelex/cypress-allure-plugin"]

Update support > e2e ts file
  - import '@shelex/cypress-allure-plugin';

## Commands to generate Allure html report
  - npx cypress run 
  - allure serve allure-results
 