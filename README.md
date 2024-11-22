# Early AI - Generate Tests - improve code quality
EarlyAI - Automatically Generate Validated and Verified Unit Tests to Improve Code Qualit.

## Features

### 1. Automatically Test Generation
With a single click, developers can generate functional tests directly within the IDE, utilizing Code Lens or the context menu for seamless integration.
![Generate-Tests](https://raw.githubusercontent.com/earlyai/earlyai-vscode-release/main/media/features/1-GenerateTests.gif "Generate Tests")

### 2. IDE Integrated
Seamless Test Generation Directly from Your Code.
![Generate-Tests-From-Code](https://raw.githubusercontent.com/earlyai/earlyai-vscode-release/main/media/features/2-GenerateTestsFromCode.gif "Generate Tests From Code")

### 3. Earl
Your AI Test Engineer does all three: generating tests, analyzing code, and writing documentation.
![Earl](https://raw.githubusercontent.com/earlyai/earlyai-vscode-release/main/media/features/6-earl.png "Earl")

### 4. Simple navigation
Developers can effortlessly navigate to newly generated tests to review and enhance them as needed.
![Goto-Tests](https://raw.githubusercontent.com/earlyai/earlyai-vscode-release/main/media/features/3-goto-tests.gif "Go To Tests")

### 5. High quality tests
EarlyAI produces comprehensive tests that include mocks and covers various scenarios, such as happy paths and edge cases, thereby improving code coverage and identifying potential bugs.

![Test-Quality](https://raw.githubusercontent.com/earlyai/earlyai-vscode-release/main/media/features/4-test-quality.gif "Test Quality")

### 6. Increased coverage
Visualize the impact of your tests on code coverage and ensure your efforts are contributing to a more robust and reliable application.
![Coverage](https://raw.githubusercontent.com/earlyai/earlyai-vscode-release/main/media/features/5-highCoverage.gif "Coverage")

## See it in  action
Visit our [sample ToDo app in github](https://github.com/earlyai/earlyai-todo-app)

## Support
### IDEs
* vsCode
### Test Frameworks
* Optiomized by using Jest and Mocha
### Languages
* JavaScript, TypeScript, Node.js, React, Angular

## Setup & Configuration

1. Prerequisites
For an easy initial setup we recommend you go through our [sample ToDo app in github](https://github.com/earlyai/earlyai-todo-app) first.

Before installing the extension, ensure you have the following prerequisites installed:
* [VSCode](https://code.visualstudio.com/download) (Version 1.88 and later)
* NodeJS
* Jest
* TypeScript
* ts-jest

You can install Jest and TypeScript typings via npm:
```
npm install --save-dev jest @types/jest ts-jest
```
Supported Test Frameworks
* Jest: This extension is currently optimized for generating unit tests with Jest.
<br>

Installation

* Search for **EarlyAI** on the Visual Studio Marketplace via the IDE or the [Web](https://marketplace.visualstudio.com/items?itemName=Early-ai.EarlyAI) and Install Early's extension 
* Ensure that your project is set up with NodeJS and Jest.

2. Configuration (Jest related)
You are ready to go if you have Jest configured and the above prerequisites installed! If not, please continue reading below for further setup instructions.

Configure Jest in your project to integrate with the extension. Below is an example of a typical Jest configuration suitable for TypeScript projects:
Filename is “jest.config.ts” and resides in the project's root folder.

```
import type { Config } from '@jest/types';
const config: Config.InitialOptions = {
  preset: 'ts-jest',
  testEnvironment: 'node',
  rootDir: 'src',
  testRegex: '.*\\.test\\.ts$',
  moduleNameMapper: {
    "^@src/(.*)$": "<rootDir>/$1"
  },
  collectCoverageFrom: ["./**/*.(t|j)s"]
};
export default config;
```
>Important Configuration Parameters:

* testEnvironment: Specifies the environment in which the tests are executed
* testRegex: make sure you have 'test" in the regex. for example if you currently have 'spec' you need to change it to something like 
```
testRegex:  ".*\\.(test)|(spec)\\.ts$"};
```
* ModuleNameMapper: If you have path aliases in tsconfig.json, identify them under compilerOptions.paths. Then, add matching regex patterns to moduleNameMapper in your Jest config to mirror the aliases, using <rootDir> to map them to their corresponding directories, like this:
Ensure your Jest configuration is properly set up to work with TypeScript and the paths align with your project structure.
