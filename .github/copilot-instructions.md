# Copilot Instructions

## Project Overview

This is a placeholder. Update this overview accordingly.

## Target Framework, Language, and Tools

- **Framework**: .NET 10.0 (`net10.0`)
- **Language Version**: Latest C# features enabled
- **Nullable Reference Types**: Enabled project-wide
- **Implicit Usings**: Enabled
- **Treat Warnings as Errors**: Enabled globally
- **Tools**: Entity Framework Core

## Project Structure

All paths from the root of the repository:
- `/src`: All source code including unit tests
- `/src/.editorconfig`: Code style and formatting configuration
- `/src/Directory.Build.props`: Shared properties for all projects
- `/src/Directory.Packages.props`: Central Package Management (CPM) configuration
- `/src/Template.slnx`: Solution file (XML format)

## General Coding Instructions

- Make only high confidence suggestions when reviewing code changes.
- Write code with good maintainability practices, including comments on why certain design decisions were made.
- Handle edge cases and write clear exception handling.
- For libraries or external dependencies, mention their usage and purpose in comments.
- Write clear and concise comments for each function.
- Write unit testable code wherever possible
- Offer to add tests to generated code if applicable

## General Testing Instructions

- Always include test cases for critical paths of the application.
- Copy existing style in nearby files for test method names and capitalization.
- Follow Arrange-Act-Assert pattern but do not emit "Act", "Arrange" or "Assert" comments.

## Security

- Follow OWASP guidelines for secure coding practices
- Validate and sanitize all user inputs
- Use parameterized queries or ORM features to prevent SQL injection
- Implement proper authentication and authorization mechanisms
- Use HTTPS for all communications
- Explain how to secure both controller-based and Minimal APIs consistently.
- Demonstrate integration with Microsoft Entra ID (formerly Azure AD).
- Show how to implement role-based and policy-based authorization.

## Documentation Conventions

- Use Markdown for all documentation files
- Use headings (`#`, `##`, `###`) to organize content
- Include code snippets with proper syntax highlighting
- Run linting tools on documentation files to ensure consistency
- Lists and code listings should always have a blank line before and after them