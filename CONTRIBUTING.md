# Contributing to ZapisAxis

Thank you for your interest in contributing to ZapisAxis! We welcome contributions from the community to help improve this Financial Management System. This guide outlines how to contribute, the process for submitting changes, and the standards we follow.

## Table of Contents

- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
- [Code Style and Standards](#code-style-and-standards)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Reporting Issues](#reporting-issues)
- [Community Guidelines](#community-guidelines)

## Getting Started

1. **Fork the Repository**:
   - Visit [https://github.com/VoxDroid/ZapisAxis](https://github.com/VoxDroid/ZapisAxis) and click the "Fork" button.
   - Clone your fork to your local machine:
     ```bash
     git clone https://github.com/YOUR_USERNAME/ZapisAxis.git
     cd ZapisAxis
     ```

2. **Set Up the Development Environment**:
   - Install [XAMPP](https://www.apachefriends.org) for MySQL and Apache.
   - Install Visual Studio with the .NET Framework 4.7.2 or higher.
   - Open the ZapisAxis solution in Visual Studio and restore NuGet packages.
   - Follow the [Installation instructions](README.md#installation) in the README to set up the database.

3. **Explore the Codebase**:
   - Familiarize yourself with the project structure, particularly key files like `Dashboard.cs`, `StudentFile.cs`, `SubBudMan.cs`, `SubTranLo.cs`, `Export.cs`, and `Login.cs`.
   - Review the [System Architecture](README.md#system-architecture) for an overview of the client-server design.

## How to Contribute

We accept contributions in the form of bug fixes, new features, documentation improvements, and more. Here are some ways to contribute:

- **Bug Fixes**: Identify and fix issues in the codebase. Check the [Issues page](https://github.com/VoxDroid/ZapisAxis/issues) for reported bugs.
- **New Features**: Propose enhancements, such as UI improvements, additional export formats, or performance optimizations.
- **Documentation**: Improve the README, add code comments, or create tutorials.
- **Testing**: Write unit tests or perform manual testing to ensure stability.

### Suggested Contributions

- Implement password hashing for user credentials (e.g., BCrypt or SHA-256).
- Add support for cloud-based MySQL hosting.
- Enhance accessibility in the UI (e.g., screen reader support).
- Optimize database queries in `ModStudFil.cs` or `ModTranLo.cs`.
- Add bulk import functionality for student records or transactions.

## Code Style and Standards

To maintain consistency, please adhere to the following guidelines:

- **C# Coding Style**:
  - Use PascalCase for class names, methods, and properties (e.g., `StudentFile`).
  - Use camelCase for local variables and parameters (e.g., `studentId`).
  - Add meaningful comments for complex logic or public methods.
  - Follow the existing structure for Windows Forms event handlers.

- **Database Queries**:
  - Use parameterized queries to prevent SQL injection (see `MySqlCommand` usage in `ModStudFil.cs`).
  - Avoid hardcoding table or column names; use constants where possible.

- **UI Design**:
  - Use Bunifu UI and Guna UI components consistently with the existing design.
  - Ensure responsive layouts for different screen resolutions.

- **Commit Messages**:
  - Write clear, concise commit messages (e.g., "Fix null reference in SubTranLo.cs").
  - Reference issue numbers if applicable (e.g., "Add export to JSON #123").

- **Testing**:
  - Test changes locally with XAMPP and MySQL.
  - Ensure no breaking changes to the database schema or existing features.

## Submitting a Pull Request

1. **Create a Branch**:
   - Create a new branch for your changes:
     ```bash
     git checkout -b feature/your-feature-name
     ```

2. **Make Changes**:
   - Implement your changes, following the [Code Style and Standards](#code-style-and-standards).
   - Test thoroughly to ensure functionality and stability.

3. **Commit Changes**:
   - Stage and commit your changes:
     ```bash
     git add .
     git commit -m "Describe your changes here"
     ```

4. **Push to Your Fork**:
   - Push your branch to your GitHub fork:
     ```bash
     git push origin feature/your-feature-name
     ```

5. **Open a Pull Request**:
   - Go to the [ZapisAxis repository](https://github.com/VoxDroid/ZapisAxis) and click "New Pull Request".
   - Select your branch and provide a detailed description using the [Pull Request Template](.github/pull_request_template.md).
   - Reference any related issues (e.g., "Closes #123").

6. **Review Process**:
   - Maintainers will review your pull request and provide feedback.
   - Be responsive to comments and make requested changes.
   - Once approved, your changes will be merged into the main branch.

## Reporting Issues

If you encounter bugs or have feature requests, please use the [GitHub Issues page](https://github.com/VoxDroid/ZapisAxis/issues):

- **Bug Reports**:
  - Describe the issue, including steps to reproduce.
  - Include screenshots, error messages, and environment details (e.g., Windows version, XAMPP version).
  - Check for existing issues to avoid duplicates.

- **Feature Requests**:
  - Explain the proposed feature and its benefits.
  - Provide use cases or examples where possible.

## Community Guidelines

We strive to create a welcoming and inclusive community. Please adhere to our [Code of Conduct](CODE_OF_CONDUCT.md) in all interactions, including issues, pull requests, and discussions.

Thank you for contributing to ZapisAxis! Your efforts help make this project better for everyone.

---