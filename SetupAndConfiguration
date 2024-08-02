



# Setup and Configuration Guide

This Visual Studio Code extension is designed to automatically generate unit tests for JavaScript and TypeScript projects using Jest. 
Below is a guide to help you install, configure, and utilize the extension effectively.

## 1. Prerequisites
For an easy initial setup, we recommend you first go through our [getting started guide](https://www.startearly.ai/docs/getting-started).
The extension supports [VSCode](https://code.visualstudio.com/download) (Version 1.88 and later).

Before installing the extension, ensure you have the following prerequisites installed:

* [VSCode](https://code.visualstudio.com/download) (Version 1.88 and later)
* NodeJS
* Jest (if Jest does not exists or not configured correctly you can still generate tests but we won't be able to validate them)
* JavaScript orTypeScript
* ts-jest

JavaScript
```
npm install jest babel-jest @babel/core @babel/preset-env --save-dev
```

TypeScript
```
npm install jest @types/jest ts-jest ts-node --save-dev
```


Supported Test Frameworks
* Jest: This extension is currently, optimized for generating unit tests with Jest.
<br>
Installation
* Search for **EarlyAI** on the Visual Studio Marketplace via the IDE or the [Web](https://marketplace.visualstudio.com/items?itemName=Early-ai.EarlyAI) and Install Early's extension 
* Ensure that your project is set up with NodeJS and Jest.

## 2. Configuration
You are ready to go if you have Jest configured and the above prerequisites installed! If not, please continue reading below for further setup instructions.

Configure Jest in your project to integrate with the extension. Below is an example of a typical Jest configuration suitable for TypeScript projects:

Typical TypeScript jest configuration. Please adjust to your settings!
```
{
  preset: 'ts-jest',
  testEnvironment: 'node',
  testMatch: ['**/?(*.)+(spec|test).ts?(x)'],
  collectCoverageFrom: [
    'src/**/*.{ts,tsx}',   // Include source files
    '!src/**/*.d.ts',   // Exclude declaration files
  ],
  coveragePathIgnorePatterns: [
    '/node_modules/', // Exclude node modules
  ],
  coverageReporters: ['text', 'lcov'],
}
```

Typical JavaScript jest configuration. Please adjust to your settings!
```
{
  testEnvironment: 'node',
  testMatch: ['**/?(*.)+(spec|test).js?(x)'],
  collectCoverageFrom: [
    'src/**/*.{js,jsx}',  // Include source files
  ],
  coveragePathIgnorePatterns: [
    '/node_modules/', // Exclude node modules
  ],
  coverageReporters: ['text', 'lcov'],
}
```

Make sure your Babel configuration includes the following settings for JavaScript (ES6+):
```
{
  presets: ['@babel/preset-env'],
}
```

>Important Configuration Parameters:
* testRegex: make sure you have 'test" in the regex. for example, if you currently have 'spec' you need to change it to something like 
```
testRegex:  ".*\\.(test)|(spec)\\.ts$"};
```
* ModuleNameMapper: If you have path aliases in tsconfig.json, identify them under compilerOptions.paths. Then, add matching regex patterns to moduleNameMapper in your Jest config to mirror the aliases, using <rootDir> to map them to their corresponding directories, like this:
Ensure your Jest configuration is properly set up to work with TypeScript and the paths align with your project structure
 
## 3. Preparing to Use the Extension
Steps to follow before generating tests:

#### 1. Activate the Extension:
* Open your TypeScript project in Visual Studio Code.
* Switch to the extension's view and complete the signup process.

#### 2. Verify Test Setup:
* Ensure you can successfully run existing tests. If tests do not run properly, you may need to adjust your Jest configuration according to the errors in the [troubleshooting section](#5troubleshooting).
* Navigate to the test explorer in the extension's sidebar and refresh the extension using the “Refresh Coverage” icon.

#### 3. update Git's ".ignore" file
* add **.early.coverage** to your git **.ignore** file 
 
## 4. Using the Extension
To effectively use the extension for generating unit tests, follow these simple steps:
#### 1. Activate the Extension:
* Open your TypeScript project in Visual Studio Code
* Switch to the extension's view
#### 2. Locate the Target Method:
* Use the extension's sidebar to navigate the tree view and find the method or function you wish to test. Currently, unit tests can be generated only to public methods/functions
#### 3. Initiate Test Generation:
* You can generate unit tests in two ways:
  <br>
a.	Click on the button next to the method name in the code explorer
b.	Click on the "Generate tests" code-lens displayed above the public method name
#### 4. Start the Test Generation Process:
* Press the 'play' button adjacent to the function or method in the tree view. This initiates the test generation
#### 5. Monitor the Process:
* A popup window will appear at the bottom right of the IDE, indicating that the test generation is underway
#### 6. Allow Time for Generation:
* The extension may take up to 60 seconds to automatically generate the necessary unit tests
#### 7. Review the Generated Tests:
* Once the tests are generated, a new file containing the tests will be automatically added to your project
 
## 5. Troubleshooting
If you encounter any issues while using the extension, consider the following steps:

* If the Tree is not populated, reload the window
* Verify Jest Configuration: Ensure that your Jest configuration matches your project setup, particularly ensuring that collectCoverage is set to true. The extension relies on Jest's coverage reports to function properly. If coverage is not being collected, the extension will not work as expected
* Check Dependencies: Make sure that all dependencies, including Jest and @types/jest, are correctly installed and up to date
* Check Extension Output: Monitor the "EarlyAI" output window within Visual Studio Code for feedback from the extension. This window displays specific error messages and diagnostics that can help identify any issues with the test generation process

If the problem persists after these checks, please consider reporting the issue on the GitHub repository with detailed information about your setup and the errors encountered.

## 6. Reporting Issues
If you encounter a bug or an issue, please report it via GitHub Issues:
1.	Visit the [GitHub](https://github.com/earlyai/earlyai-vscode-release/issues) repository
2.	Navigate to the 'Issues' section
3.	Click on 'New Issue'
4.	Provide a descriptive title and a detailed description of the issue. Attach screenshots or error logs, if possible, to help us understand the problem better
5.	Submit the issue
## 7. Suggesting Enhancements
**We are always looking for ways to make our product more powerful:**
1.	Visit the [GitHub](https://github.com/earlyai/earlyai-vscode-release/issues) repository
2.	Go to the 'Issues' section and check if a similar enhancement has already been proposed
3.	If not, create a new issue by selecting the 'Feature request' template
4.	Describe your idea with as many details as possible, explaining how it would benefit our users
5.	Submit the request


**Looking forward to hearing from you**
**The Early team.**
