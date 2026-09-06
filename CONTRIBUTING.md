# Contributing to My Agent Demo

Thank you for considering contributing to **My Agent Demo**! We appreciate your help in making this project better. Please follow these guidelines to streamline the contribution process.

## Getting Started

1. **Fork the repository** on GitHub.
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/<your-username>/my-agent-demo.git
   cd my-agent-demo
   ```
3. **Create a new branch** for your work:
   ```bash
   git checkout -b <feature-or-bugfix-name>
   ```
4. **Set up the development environment** (see the [README](README.md) for details).

## Development Workflow

- **Make small, focused commits**. Each commit should represent a single logical change.
- **Write tests** for new functionality or bug fixes. Tests live in the `tests/` directory.
- **Run the test suite** before committing:
  ```bash
  pytest
  ```
- **Follow code style**: we use `ruff` and `black`. Run them with:
  ```bash
  ruff check .
  black .
  ```

## Submitting a Pull Request

1. Push your branch to your fork:
   ```bash
   git push origin <feature-or-bugfix-name>
   ```
2. Open a **Pull Request** (PR) on the original repository.
3. Fill out the PR template, providing:
   - A clear description of the changes.
   - Motivation and context.
   - Any relevant issue numbers (e.g., `Closes #42`).
4. Ensure all **CI checks pass**.
5. Request a review from the maintainers.

## Code of Conduct

Please note that this project adheres to a [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## Reporting Issues

If you encounter a bug or have a feature request, please open an issue on GitHub. Include:
- A clear title.
- Steps to reproduce (for bugs).
- Expected vs. actual behavior.
- Any relevant logs or screenshots.

## License

By contributing, you agree that your contributions will be licensed under the project's MIT License.
