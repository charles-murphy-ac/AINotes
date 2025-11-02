# Repository Guidelines

## Project Structure & Module Organization

- `src/`: Core application modules
- `tests/`: Unit and integration tests
- `docs/`: Project documentation
- `scripts/`: Development and deployment utilities
- `config/`: Configuration files

## Build, Test, and Development Commands

- `pytest tests/`: Run all tests
- `black src/`: Format Python code
- `mypy src/`: Run static type checking
- `python -m src.main`: Launch application

## Coding Style & Naming Conventions

- Follow PEP 8 style guide
- 4-space indentation (no tabs)
- Use descriptive snake_case names
- Class names in PascalCase
- Format with Black (line length: 88)
- Type annotations for all function signatures

## Testing Guidelines

- pytest framework
- Tests mirror src structure (`tests/test_module.py`)
- Test names: `test_<method>_<condition>`
- Aim for 80%+ coverage
- Use fixtures for common test setup

## Commit & Pull Request Guidelines

- Imperative mood commit messages (`"Add feature"`, not `"Added feature"`)
- Reference issues: `"Fix #123 - description"`
- PRs require:
    - Description of changes
    - Linked GitHub issue
    - Passing CI checks
    - Approval from 1 maintainer

## Security & Configuration Tips

- Never commit secrets (use .env for local config)
- Validate all user input
- Use parameterized queries for database access