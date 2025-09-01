# Contributing to dsllm

Thank you for your interest in contributing to dsllm! This document provides guidelines and information for contributors.

## Development Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/frenkd/dsllm.git
   cd dsllm
   ```

2. **Install in development mode**:
   ```bash
   pip install -e .[dev]
   ```

3. **Install pre-commit hooks**:
   ```bash
   pre-commit install
   ```

## Development Workflow

1. **Create a branch** for your feature or fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes** following the code style guidelines

3. **Run tests**:
   ```bash
   pytest tests/ -v
   ```

4. **Run linting**:
   ```bash
   black src/ tests/
   isort src/ tests/
   flake8 src/ tests/
   mypy src/
   ```

5. **Commit and push** your changes

6. **Create a pull request** with a clear description of your changes

## Code Style

- Follow PEP 8 guidelines
- Use Black for code formatting
- Use isort for import sorting
- Type hints are required for all public APIs
- Docstrings should follow Google style

## Testing

- Write tests for all new functionality
- Maintain or improve test coverage
- Tests should be clear and well-documented
- Use pytest fixtures for common test setup

## Areas for Contribution

### High Priority
- Additional DSL generators (GraphQL, MongoDB, etc.)
- New LLM providers (Anthropic, Google, etc.)
- Enhanced validation and error handling
- Performance improvements

### Medium Priority
- Documentation improvements
- Example applications
- Integration with popular frameworks
- CLI interface

### Future Features
- Agentic loops and self-correction
- Automated testing and validation
- Observability and monitoring
- Caching and optimization

## Pull Request Guidelines

- Keep PRs focused and atomic
- Include tests for new functionality
- Update documentation as needed
- Ensure CI passes
- Provide clear commit messages

## Questions or Issues?

- Open an issue for bugs or feature requests
- Start a discussion for design questions
- Check existing issues before creating new ones

Thank you for contributing to dsllm!
