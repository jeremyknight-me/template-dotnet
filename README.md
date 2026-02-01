# template-dotnet

A template repository for dotnet applications.

## Repository Structure

```
├── .github/          # GitHub workflows, AI instructions, etc.
├── decisions/        # Architectural decision records
├── src/              # Application source code and projects
    ├── Directory.Build.props    # Central MSBuild properties for all projects
    ├── Directory.Packages.props # Central Package Management configuration
    └── Template.slnx            # Solution file
├── README.md
```

## Development Guidelines

This repository follows conventions defined in [AGENTS.md](AGENTS.md), including:

- **Central Package Management**: All package versions managed in [Directory.Packages.props](Directory.Packages.props)
- **Code Style**: 2-space indentation, file-scoped namespaces, Allman-style braces
- **Testing**: xUnit framework with Arrange-Act-Assert pattern
- **Warnings as Errors**: All compiler warnings must be addressed

Run `dotnet format` to automatically format code according to project conventions.

## Contributing

1. Create a feature branch from `main`
2. Make your changes following the coding conventions
3. Ensure all tests pass (`dotnet test`)
4. Submit a pull request
