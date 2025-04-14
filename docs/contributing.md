# Contributing

Thank you for considering contributing to the **mkdocs-curriculum-vitae** project! We appreciate your time and effort in helping to make this project better. Below are some guidelines to help you get started.

## 📜 Table of Contents

- [🚀 How Can I Contribute?](#how-can-i-contribute)
    - [🐛 Reporting Bugs](#reporting-bugs)
    - [💡 Suggesting Enhancements](#suggesting-enhancements)
    - [🔄 Pull Requests](#pull-requests)
- [🛠️ Setting Up the Development Environment](#setting-up-the-development-environment)
    - [🌐 Using Gitpod](#using-gitpod)
    - [💻 Local Development](#local-development)
- [📝 Coding Guidelines](#coding-guidelines)
- [📄 License](#license)

## 🚀 How Can I Contribute?

### 🐛 Reporting Bugs

If you find a bug, please report it by creating an issue on our [GitHub Issues](https://github.com/Paul-Riviere/mkdocs-curriculum-vitae/issues) page. Provide detailed information to help us understand the problem and how to reproduce it.

### 💡 Suggesting Enhancements

We welcome suggestions for new features or improvements. To suggest an enhancement, please open an issue on our [GitHub Issues](https://github.com/Paul-Riviere/mkdocs-curriculum-vitae/issues) page, clearly explaining the enhancement and how it could benefit the project.

### 🔄 Pull Requests

If you'd like to contribute code, please follow these steps:

- **Fork the repository** to your GitHub account.
- **Clone your fork** to your local machine:
```sh
git clone https://github.com/your-username/mkdocs-curriculum-vitae.git
```
- **Create a new branch** for your feature or bugfix:
```sh
git checkout -b feature/your-feature-name
```
- **Make your changes** and commit them with clear and concise commit messages (please use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)).
```sh
git add . && git commit -m "feat: my new feature"
```
- **Push your branch** to your forked repository:
```sh
git push origin feature/your-feature-name
```
- **Open a Pull Request** on the main repository, describing your changes in detail.

Please ensure your code follows the project's [coding guidelines](#coding-guidelines) and includes appropriate tests.

## 🛠️ Setting Up the Development Environment

To set up the development environment for `mkdocs-curriculum-vitae`, **fork the repository** to your GitHub account.

### 🌐 Using Gitpod

You can start developing the project in an online environment using [Gitpod](https://gitpod.io).

Please read the official [Getting started](https://www.gitpod.io/docs/introduction/getting-started) from Gitpod documentation and choose your forked project.

### 💻 Local Development

If you prefer to set up the project on your local machine, follow these steps:

- Install dependencies.
    - Python (tested with 3.12.4)
    - [Task](https://taskfile.dev/) (tested with 3.35.1)
- Clone the forked repository:
```sh
git clone https://github.com/your-username/mkdocs-curriculum-vitae.git
```
- Run the bootstrap command:
```sh
task bootstrap
```

- When you're done, please run the test doc using the task command, and in another shell run the task command to generate screenshots:
```sh
# Shell 1
task mkdocs:serve-test-doc
# Shell 2
task documentation:generate-screenshots
```

## 📝 Coding Guidelines

Please follow these coding standards when contributing:

- PEP 8 for Python code.
- Write clear and descriptive commit messages (please use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)).
- Include tests for any new functionality or bug fixes.
- Update the documentation as soon as possible.
- Ensure that all tests pass before submitting a pull request.

## 📄 License

By contributing, you agree that your contributions will be licensed under the project's [MIT License](https://github.com/Paul-Riviere/mkdocs-curriculum-vitae/blob/main/LICENSE).
