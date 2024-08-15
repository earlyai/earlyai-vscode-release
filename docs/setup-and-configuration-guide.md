# Setup and Configuration Guide

This Visual Studio Code extension is designed to automatically generate unit tests for JavaScript and TypeScript projects using Jest, Mocha, Sinon, and Chai. Below is a guide to help you install, configure, and utilize the extension effectively.

## Index
1. [Prerequisites](#1-prerequisites)
2. [Installation](#2-installation)
3. [Configuration](#3-configuration)
    - [Jest](#jest)
    - [Mocha](#mocha)
4. [Preparing to Use the Extension](#4-preparing-to-use-the-extension)
5. [Using the Extension](#5-using-the-extension)
6. [Troubleshooting](#6-troubleshooting)
7. [Reporting Issues](#7-reporting-issues)
8. [Suggesting Enhancements](#8-suggesting-enhancements)

## 1. Prerequisites
For an easy initial setup, we recommend you first go through our [getting started guide](https://www.startearly.ai/docs/getting-started). The extension supports [VSCode](https://code.visualstudio.com/download) (Version 1.88 and later).

Before installing the extension, ensure you have the following prerequisites installed:

- [VSCode](https://code.visualstudio.com/download) (Version 1.88 and later)
- NodeJS
- JavaScript or TypeScript

## 2. Installation
### Installing the Extension
- Search for **EarlyAI** on the Visual Studio Marketplace via the IDE or the [Web](https://marketplace.visualstudio.com/items?itemName=Early-ai.EarlyAI) and install Early's extension.
- Ensure that your project is set up with NodeJS and Jest or Mocha.

## 3. Configuration
### Jest
#### JavaScript
- prerequisites
```bash
npm install jest babel-jest @babel/core @babel/preset-env --save-dev
```
- Typical JavaScript Jest Configuration
```json
{
  "testEnvironment": "node",
  "testMatch": ["**/?(*.)+(spec|test).js?(x)"],
  "collectCoverageFrom": ["src/**/*.{js,jsx}"],
  "coveragePathIgnorePatterns": ["/node_modules/"],
  "coverageReporters": ["text", "lcov"]
}
```
#### TypeScript
- prerequisites
```bash
npm install jest @types/jest ts-jest ts-node --save-dev
```
- Typical TypeScript Jest Configuration
```json
{
  "preset": "ts-jest",
  "testEnvironment": "node",
  "testMatch": ["**/?(*.)+(spec|test).ts?(x)"],
  "collectCoverageFrom": ["src/**/*.{ts,tsx}", "!src/**/*.d.ts"],
  "coveragePathIgnorePatterns": ["/node_modules/"],
  "coverageReporters": ["text", "lcov"]
}
```
### Mocha
#### JavaScript
- prerequisites
```bash
npm install mocha chai sinon --save-dev
```
- Typical JavaScript Mocha Configuration
```json
{
  "spec": "src/**/*.spec.js"
}
```
#### TypeScript
- prerequisites
```bash
npm install mocha @types/mocha chai @types/chai sinon @types/sinon ts-node --save-dev
```
- Typical TypeScript Mocha Configuration
```json
{
  "require": "ts-node/register",
  "spec": "src/**/*.spec.ts"
}
```
## 4. Preparing to Use the Extension

- Steps to Follow Before Generating Tests

1. Activate the Extension:
   - Open your TypeScript or JavaScript project in Visual Studio Code.
   - Switch to the extension’s view and complete the signup process.
2. Verify Test Setup:
   - Ensure you can successfully run existing tests. If tests do not run properly, you may need to adjust your Jest or Mocha configuration according to the errors in the troubleshooting section.
   - Navigate to the test explorer in the extension’s sidebar and refresh the extension using the “Refresh Coverage” icon.
3. Update Git’s “.ignore” file:
   - Add .early.coverage to your git .ignore file.


## 5. Using the Extension

- Steps to Generate Unit Tests

1. Activate the Extension:
   - Open your TypeScript or JavaScript project in Visual Studio Code.
   - Switch to the extension’s view.
2. Locate the Target Method:
   - Use the extension’s sidebar to navigate the tree view and find the method or function you wish to test.
3. Initiate Test Generation:
   - Click on the button next to the method name in the code explorer or the “Generate tests” code lens displayed above the public method name.
4. Start the Test Generation Process:
   - Press the ‘play’ button adjacent to the function or method in the tree view.
5. Monitor the Process:
   - A popup window will appear at the bottom right of the IDE, indicating that the test generation is underway.
6. Allow Time for Generation:
   - The extension may take up to 60 seconds to automatically generate the necessary unit tests.
7. Review the Generated Tests:
   - Once the tests are generated, a new file containing the tests will be automatically added to your project.

## 6. Troubleshooting

If you encounter any issues while using the extension, consider the following steps:

- Check Dependencies: Make sure that all dependencies, be it Jest or Mocha, and their types, are correctly installed and up to date.
- Tree Not Populated: Reload the window.
- Coverage is not displayed - this feature is available for Jest only. Please ensure your configuration matches your project setup, particularly that collectCoverageFrom covers the entire testable code.
- Check Extension Output: Monitor the “EarlyAI” output window within Visual Studio Code for feedback from the extension.

If the problem persists after these checks, please report the issue on the GitHub repository with detailed information about your setup and the errors encountered.

## 7. Reporting Issues

If you encounter a bug or an issue, please report it via GitHub Issues:

1. Visit the GitHub repository issues [here](https://github.com/earlyai/earlyai-vscode-release/issues).
2. Select ‘New Issue’.
3. Enter a clear title and a detailed description of the issue. If possible, include screenshots or error logs to assist us in understanding the problem.
4. Submit the issue.

## 8. Suggesting Enhancements

We are always looking for ways to make our product more powerful:

1. Visit the GitHub repository issues section [here](https://github.com/earlyai/earlyai-vscode-release/issues).
2. Check if a similar enhancement has already been proposed.
3. If not, create a new issue by selecting the ‘Feature request’ template.
4. Describe your idea with as many details as possible, explaining how it would benefit our users.
5. Submit the request.

Looking forward to hearing from you,

The Early team.
 
