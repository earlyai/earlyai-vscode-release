# Changelog

## 1.3.1

This update includes a few important fixes to improve the Python experience:
 
1. Coverage Display Fixed
Resolved an issue where coverage wasn’t shown for Python files.
2. Python Enabled for New Users
New users now have Python support turned on by default — no extra steps needed.
3. Auto-Refresh Coverage
Python coverage is now automatically refreshed after generating tests, giving you immediate feedback.

## 1.3.0

1.	📊 Python Coverage in the Tree View
You can now see test coverage indicators for Python files and folders directly in the extension’s tree view. Quickly identify what’s tested and where coverage is missing — visually, at a glance.
2.	🧪 Enhance Tests Now Supports Python
Our powerful Enhance Tests feature — previously available for JavaScript and TypeScript — is now fully supported for Python! Expand and refine your existing Python tests with ease.
3.	🧠 Earl Displays Python Tests
Earl, your AI test engineer, now shows generated Python tests in the right-hand panel, just like with JS/TS. Review them, copy them, or use them to dig deeper into your test coverage.
4.	💡 Quality Enhancements for TypeScript and JavaScript
   ✅ Mock Cleanup: We now comment out valid mocks correctly and clean up grey (untestable) tests to keep your test files neat.
   ⚛️ Deeper React Integration: Support for React components has improved with 2-level depth analysis, helping generate more meaningful tests for nested structures.


## 1.2.1

1. 🧪 Pull Request Support for Python
The Pull Request feature now supports Python projects! When you’re working on a feature branch, Early AI compares your changes against the main branch to highlight only what matters. With a focused view of your modified code, you can generate targeted unit tests and keep your Python codebase robust — without the manual effort.
2. ⚡ Smaller & Faster Extension
We’ve trimmed down the extension’s size and boosted performance. Expect faster load times, a lighter footprint, and an overall smoother experience in your IDE.

## 1.2.0

1. 🧠 Custom Test Instructions – You’re in Control!
We’ve just supercharged test generation. You can now add your own custom instructions to guide how unit tests are generated — ask for specific test cases, enforce coding styles, or request particular libraries.
Want these preferences to persist? No problem — your instructions can be saved per repository. More control, better tests, your way.
2. 💡 Better JavaScript Test Quality
We’ve fine-tuned our JS test generation engine. Expect smarter, more maintainable code that aligns with real-world expectations.
3. 🔔 Sleeker Notifications Area
The notification UI got an upgrade — now clearer and easier to follow, so you never miss out on what’s new.
4. 🐍 Python Test Stability Boost
Python unit test generation is now more robust and reliable, especially for complex or edge-case code structures.
 

## 1.1.1

1. 🧠 Major Model Upgrade – More and Better Tests!
We’ve taken a huge leap forward! Our upgraded model now generates more unit tests, with higher accuracy and better coverage — helping you catch more bugs, faster. This is a big quality boost — and we’re just getting started!

2. 🔔 Revamped Notifications Area
We redesigned the notifications panel to make it cleaner, easier to read, and more intuitive — so you never miss important updates.

3. 🛠️ Smarter TypeScript Mocks
In TypeScript unit tests, mock return types are now more realistic and accurate — making your generated tests even closer to production behavior.

4. 🐛 Minor Bug Fixes & Performance Improvements
We’ve polished a few edges and tuned the engine for a smoother, faster experience.

## 1.1.0

 
1. 🔁 Pull Request Enhancements
You can now configure the destination branch in the Pull Request view — making it easy to compare changes between branches and generate focused tests.

2. 🧪 Smarter Test Generation for Python & TypeScript
We’ve improved the code quality of generated tests for both Python and TypeScript — more accurate, more useful, and easier to maintain.

3. 🎨 UI Improvements - Subtle but impactful:
New icons for test generation and custom test generation
Smoother experience for Python users while the extension prepares to load

4. 🐛 Bug Fixes
We’ve squashed a few bugs to make everything run smoother.
 

## 1.0.0

1. 🚀 Smarter Test Generation
Major improvements to our TypeScript and Python generators mean better, cleaner, and more accurate test code out of the box.
2. 🔔 Notification Center
Look for the new bell icon next to the settings cog! It’s your new hub for feature announcements, tips, and important updates — all in one place.
3. 📂 Pull Request Tab
Working on a feature branch? Check the new “Pull Request” tab to easily view the files you’ve changed and focus your test generation where it matters most.
4. 💬 Join the Conversation
You’ll now see a link to join our Slack channel — a place where your voice matters. Share feedback, ask questions, and help shape the future of Early AI.
5. ✨ Sleek New Login Screen
We gave the sign-in flow a fresh look — faster, smoother, and nicer to look at.
6. 🧪 Smarter Test Enhancement
After tests are generated, head to the right pane to enhance them. Use a prompt to add more tests or tweak existing ones to better fit your needs.

## 0.5.30
- sign-in bug fix - we handled an issue where sometimes the sign-in process failed to update vsCode.

## 0.5.29
1. 🛠️ Generate Test Options
Alongside the familiar magic wand icon, there’s now a new wand with a cog — “Generate Test Options.” Click it to configure how tests are generated before running the request.
2. ✨ Enhanced “Enhance Tests”
Previously, enhancing a test would create a new file each time. Now, you can choose to override the most recently generated test file keeping things clean and avoiding clutter.
3. 🐍 Smarter Python Support
Python function discovery has leveled up! We now support modules inside packages within your project, making sure more of your Python code is testable out of the box.
4. Streamlined Sign-In Flow
Right after installing the extension, you’ll now see a friendly VSCode notification prompting you to sign in. Choose quick GitHub authentication or explore all options via the additional sign in options.

## 0.5.28
- Personalize your tests after they are created using Earl in the side panel.
- Improved indication of free daily capacity.
- Bug fixes.

## 0.5.27

### New Feature: Make These Tests Even Better!

We’ve added a powerful new way to customize your generated tests!

After generating tests, you’ll now see a prompt area in the side pane where you can guide us to enhance or modify the tests. Whether you want to improve coverage, restructure the test layout, or handle additional scenarios—just tell us what you need.

🧠 What you can do:
• Add edge cases or error handling
• Refactor to use beforeEach or parameterized tests
• Improve mock structure and assertions
• Use spies or test different failure modes
• Adjust test style to match your team’s patterns

## 0.5.26

- Performance improvements
- Bug fixes

## 0.5.25

- Enhanced Python server stability
- Added pro feature to generate tests for all functions in a file

## 0.5.24

- Enhanced stability of the Python service through improved exception handling and resource management.
- Streamlined Jest verification execution with optimized test runners and reduced time-to-completion.
- Implemented usage tracking for test generation.

## 0.5.23

- Improve Python server stability.

## 0.5.22

- Improve coverage calculation.
- Improve JS and TS nested classes test generation.

## 0.5.21

- Support the Windsurf IDE.
- Improved Common javascript support.

## 0.5.20

- Earl - Magically help users fix their configuration issues

## 0.5.19

- Improve TS React tests.
- Improve Python tests.

## 0.5.18

- New: PRO plan fro increased capacity and features.
- Tests indication in Earl
- React Typescripts test improvements

## 0.5.17

- Improved TS React testing support
- Improved test validation command

## 0.5.16

- Ongoing bug fixes and improvements

## 0.5.15

- User setting - new and improved design

## 0.5.14

- Add a link to the Profile Page
- Ongoing unit test improvements

## 0.5.12

- Python bug fixes and improvements

## 0.5.11

- Vtest support - support generation of tests using the vtest framework.
- Initial Python support - support generation of tests for python.

## 0.5.10

- Performance improvements

## 0.5.9

- Enable login using Google and Github

## 0.5.8

- File view improvements.
- Improved package imports in test files.

## 0.5.7

- Fix coverage tree edge cases

## 0.5.6

- Coverage tree improvements

## 0.5.5

- Improve memory consumption during test generation.

## 0.5.3

- Enhanced stability and resolved known issues for a smoother experience.

## 0.5.2

- Extend the support for React unit tests.
- Support Kebab case unit test file names.
- Earl - imporve actions.

## 0.5.1

- Minor UI changes to boost the experience.

## 0.5.0

Meet Earl – Early AI’s Quality Engineer

We’re excited to introduce Earl, our new AI-powered assistant! Earl brings two powerful new features to assist you during test generation:

- Function Documentation: Automatically generates comprehensive documentation for your functions, which you can either copy or directly insert into your code.
- Function Code Improvements: Offers suggestions to enhance your function’s code. These improvements can be easily copied for quick adjustments.

Earl works seamlessly behind the scenes while your tests are being generated, helping you improve both code quality and clarity with minimal effort!

## 0.4.42

- New “Generate Tests” Icon: We’ve added a magic wand icon to make generating tests even more fun and intuitive!
- Various stability improvements for a smoother experience.

## 0.4.41

- Fixed a bug related to removing errored imports for smoother code handling.

## 0.4.40

- Bug fixes and performance improvements.

## 0.4.39

- Enhanced React support, especially for React hooks. Unit tests now include more advanced and complex mocks for better coverage.

## 0.4.38

- Fixed bugs related to React support for a smoother and more reliable experience.

## 0.4.37

- You can now invite a friend! Use the menu in the extension to send an invite and share the benefits of using this powerful tool together.
- Some minor bug fixes.

## 0.4.36

- Some bugs have been identified and squashed.
- Imports are better created in your test files.
- "Go to tests" from the code lens behaves nicer.

## 0.4.35

- We’ve implemented significant bug fixes and performance enhancements to improve overall stability and speed.

Sneak peek: Thanks to feedback from our awesome users, we’re working on adding React support in an upcoming release. We can’t wait to share it with you—stay tuned!”

## 0.4.34

- Bug fixes and performance improvements.

## 0.4.33

- Updated .gitignore to automatically include Early’s coverage folder.

## 0.4.32

- Test generation works even faster now.
- We identified and crashed the cause for scenarios where tests were not displayed.

## 0.4.31

- Bug fixes and performance improvements.

## 0.4.30

- We identified and resolved several issues that were affecting the generation of tests for TypeScript and JavaScript projects. These fixes should improve the overall experience for our users.

## 0.4.29

- After adding support for Mocha, we’ve squashed some bugs to enhance the user experience. Happy coding.

## 0.4.28

- Mocha Support
  We’re expanding our horizons! Now you can generate tests with Mocha too, alongside Jest.
- Test Location Flexibility
  Choose your vibe - tests can now be placed as “Root” in addition to “Sibling” right next to your source folder. More options, more control.
- Custom Test File Format
  Whether you’re team test or spec, we’ve got you covered. Pick your preferred format for test files.
- Sleek New Settings Screen
  Tailor your testing experience like never before! Select your testing framework (Jest or Mocha), decide your test location (Root or Sibling), and choose your file format (spec or test) with ease.
- VSCode Insider & VSCodium Support
  We’ve got you no matter where you code! EarlyAI now plays nicely with VSCode Insider and VSCodium.

## 0.4.27

- Testable code tree - discovery improvements.

## 0.4.26

- General fixes and stability improvements to the testable code tree.

## 0.4.25

### Features

- JavaScript Test Generation Support
  We are excited to announce that our tool now supports creating tests for JavaScript code! This highly requested feature enables developers to generate unit tests for their JavaScript projects seamlessly.

## 0.4.24

### Features

- Tests are organized into test folders, sibling to the tested code.

## 0.4.23

### Features

- Effortless Test Generation: Now seamlessly supports monorepos and projects not fully configured with Jest, accessible via CodeLens or the extension tree.

## 0.4.22

### Features

- "MY CODE" - check out the tab that gives you focus on you current feature. It has Code coverage now.

## 0.4.21

### Fixes

- On-boarding now displays better assistance in setup & configuration.

### known issues

- If you don't have any tests, create them in the code lens and "Reload" once done.

## 0.4.20

### Features

- "Generate Tests" and "Goto Tests" are now available from the extension UI, Code lens, and context menu.
- You now have nice in-progress and queued indicators for "Generate Tests" operations.

## 0.4.19

### Features

- Code lens and context menu are supported for all actions. Generate tests and find your unit tests directly from the code lens or context menu.

## 0.4.18

### Features

- Introducing "My View" - focus on what matters when creating your tests. This view will display files that are changed in git (your future PR).

## 0.4.17

### Features

- Generating tests will always give you unit tests (even if it has some errors).

## 0.4.17

### Features

- We have changed some icons for better clarity.
- The mocks have been improved.

## 0.4.15

### Features

- Onboarding became easier.
- Better testable code discovery.
- Improvements when using on Windows operating system.

## 0.4.14

### Features

- Support for exporting an object with methods

## 0.4.13

### Features

- Test Navigation
- Performance optimization

## 0.4.12

### Features

- Smoother onboarding

## 0.4.11

### Features

- Quality of life

## 0.4.10

### Features

- Support macOS and Windows
- Easier onboarding

## 0.4.9

### First Release - Alpha

- First Release - Alpha
