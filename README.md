# <img src="https://playwright.dev/img/playwright-logo.svg" width="100" height="100"> Front-End, API and Visual Automation using Playwright
## Version
v1.0

## Introduction

The purpose of this project is to provide a real world template to perform Front-End, API and Visual testing using Playwright.

## Tech Stack

- TypeScript
- Playwright
- Allure
- DotEnv

## Project Structure
```
├── API            # Main Page Object Model folder.
│   ├── classes             # All the API classes and methods.
│   ├── data                # Data provider files.
│   ├── tests               # API Tests are located here.
│   └── ...                 
├── page-objects            # Main Page Object Model folder for the Front-End tests.
│   ├── data                # Data provider files.
│   ├── pages               # Page Objects.
│   ├── tests               # Front-End Tests are located here.
│   └── ...
└── .gitignore
└── README.md
└── package-lock.json
└── package.json
└── playwright.config.ts
└── .env
```

## Pre-requisites

1. Node.js (latest version).
2. VSCode (highly recommended).
3. Playwright Test for VSCode Extension (highly recommended).


## Project Setup

1. Clone this repository.
2. Go to the repository folder.
3. Run the ```npm install``` command on the terminal.
4. Create a .env file at root level with the following variables:
```
EMAIL=your@email.com
PASSWORD=your_password
BASE_URL=https://trello.com/
API_BASE_URL=https://api.trello.com/1/
API_KEY=your_api_key
API_TOKEN=your_token
```
5. Create a new Trello account.
6. Create new board called "Test Board".
7. Make sure the board has the following columns: To Do, Doing, Done.

## Dependencies
- @playwright/test
- allure-playwright
- dotenv

## Scripts
- ```cards```: Runs all the front-end cards tests on chromium, firefox and webkit: headed mode.
- ```cards-chromium```: Runs all the front-end cards tests on chromium: headed mode.
- ```cards-headless```: Runs all the front-end cards tests on chromium: headless mode.
- ```cards-allure```: Runs all the front-end cards tests on chromium: headless mode, using the Allure reporter.
- ```cards-debug```: Runs all the front-end cards tests on chromium: debug mode.
- ```cards-api```: Runs all the API cards tests.
- ```boards-api```: Runs all the API boards tests.
- ```api```: Runs all the API tests.
- ```api-html```: Runs all the API tests using the HTML reporter
- ```visual```: Runs all the Visual tests.
- ```visual-firefox```: Runs all the Visual tests on firefox: headed.
- ```visual-allure```: Runs all the Visual tests on chromium: headed, using the Allure reporter.
- ```code-gen```: Runs the code generator mode.
- ```storage-state```: Runs the Storage State login test.
- ```visual```: Runs all the Visual tests.
- ```html```: Launches the generated HTML report.
- ```allure```: Launches the generated Allure report.
