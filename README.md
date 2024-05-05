<div align="center">

# Early-AI

---

The ultimate tool for enhancing code quality and coverage - Early AI

---

Early-AI is a cutting-edge software development tool designed to boost the efficiency and quality of your code. Utilizing generative AI, it generates unit tests in real time, enhancing your coding accuracy and reducing errors. Perfect for developers looking to streamline their workflow, Early-AI offers a suite of tools that integrates seamlessly into existing development environments.
<br>
<strong>It supports Typescript with Jest</strong>

</div>

---

<br></br>

# Features

* <strong>Automatic Test Generation</strong>
  <br> Automatically generates unit tests for TypeScript code, helping developers save time and ensure thorough testing coverage.

* <strong>Visual Coverage Mapping</strong>
  <br> Displays a visual tree of code coverage, allowing developers to easily identify tested and untested parts of the codebase.
* <strong>Integration with Jest</strong>
  <br> Seamlessly integrates with Jest, the popular testing framework, ensuring compatibility and ease of use within existing projects. <br>
* <strong>CodeLens Integration</strong>
  <br> Utilize CodeLens in Visual Studio Code to quickly generate and navigate to unit tests directly from the source code, enhancing workflow efficiency.

# Setup and Configuration Guide

This Visual Studio Code extension is designed to automatically generate unit tests for TypeScript projects using Jest. Below is a guide to help you install, configure, and utilize the extension effectively.

## Prerequisites
Before installing the extension, ensure you have the following prerequisites installed:
- NodeJS
- Jest
- TypeScript

You can install Jest and TypeScript typings via npm:

```bash
npm install --save-dev jest @types/jest
```

## Supported Test Frameworks
- **Jest**: This extension is currently optimized for generating unit tests with Jest.

## Installation
- Install the extension from the Visual Studio Code Marketplace.
- Ensure that your project is set up with NodeJS and Jest.

## Configuration
Configure Jest in your project to integrate with the extension. Below is an example of a typical Jest configuration suitable for TypeScript projects:

```javascript
module.exports = {
  // Basic Environment Setup
  testEnvironment: "node",
  rootDir: "src",

  // Module Resolution
  moduleFileExtensions: ["js", "json", "ts"],
  transform: {
    "^.+\\.(t|j)s$": "ts-jest"
  },
  moduleNameMapper: {
    "^@src/(.*)$": "<rootDir>/$1"
  },

  // Testing Patterns and Coverage
  testRegex: ".*\\.test\\.ts$",
  collectCoverage: true,
  collectCoverageFrom: ["**/*.(t|j)s"],
  coverageDirectory: "../coverage",
};
```

## Important Configuration Parameters:
- <strong>testEnvironment</strong>: Specifies the environment in which the tests are executed.
- <strong>collectCoverage</strong>: Enables the collection of code coverage information.
- <strong>collectCoverageFrom</strong>: Defines the files for which coverage information should be collected.
- <strong>coverageDirectory</strong>: Specifies the directory where coverage reports will be stored.

Ensure your Jest configuration is properly set up to work with TypeScript and the paths align with your project structure.

## Using the Extension
To effectively use the extension for generating unit tests, follow these simple steps:

1. **Activate the Extension**: Open your TypeScript project in Visual Studio Code and switch to the extension's view.
2. **Select a Function or Method**: In the extension's sidebar, navigate through the tree view to locate the method or function for which you want to create unit tests.
3. **Generate Tests**: Click the 'play' button next to the function or method in the tree to start the test generation process.
4. **Test Generation**: Allow the extension some time to automatically generate the necessary unit tests.
5. **Review the Tests**: Once the tests are created, a new file containing the generated tests will be automatically added to your project.

## Troubleshooting
If you encounter any issues while using the extension, consider the following steps:

- <strong>Verify Jest Configuration</strong>: Ensure that your Jest configuration matches your project setup, particularly ensuring that collectCoverage is set to true. The extension relies on Jest's coverage reports to function properly. If coverage is not being collected, the extension will not work as expected.
- <strong>Check Dependencies</strong>: Make sure that all dependencies, including Jest and @types/jest, are correctly installed and up-to-date.
- <strong>Check Extension Output</strong>: Review the output from the extension in its dedicated output window within Visual Studio Code. This output can provide specific error messages and clues about what might be going wrong.

If the problem persists after these checks, please consider reporting the issue on the GitHub repository with detailed information about your setup and the errors encountered.

## Reporting Issues
If you encounter a bug or an issue, please report it via GitHub Issues:

1. Visit the GitHub repository.
2. Navigate to the 'Issues' section.
3. Click on 'New Issue'.
4. Provide a descriptive title and a detailed description of the issue. Attach screenshots or error logs if possible to help us understand the problem better.
5. Submit the issue.

## Suggesting Enhancements
We are always looking for ways to make our extension more useful:

1. Visit the GitHub repository.
2. Go to the 'Issues' section and check if a similar enhancement has already been proposed.
3. If not, create a new issue by selecting the 'Feature request' template.
4. Describe your idea with as many details as possible, explaining how it would benefit users of the extension.
5. Submit the request.
