# 🌟Awesome Precommit

A curated list of awesome pre-commit hooks, tools, and resources to improve your development workflow.

------

## 📃Table of Contents

1. [Introduction](#ℹ️Introduction)
2. [Languages](#languages)
3. [Contributing](#contributing)
4. [License](#%EF%B8%8Flicense)

## ℹ️Introduction

Welcome to **Awesome Precommit**! This repository is a curated collection of pre-commit hooks, tools, and resources designed to help developers automate and improve their workflows. Whether you're working on a small personal project or a large-scale team effort, pre-commit hooks can save you time, enforce coding standards, and catch errors before they make it into your codebase.

This list includes hooks for linting, formatting, security checks, documentation, testing, and more. Contributions are welcome, so feel free to suggest new hooks or improvements!

### What is Pre-commit?

Pre-commit is a framework for managing and maintaining multi-language pre-commit hooks. These hooks are scripts or tools that run automatically before you commit code to your repository. They help enforce coding standards, catch errors, and ensure consistency across your codebase.

### Why Use Pre-commit?

- **Automate Code Quality Checks**: Run linters, formatters, and other tools automatically.
- **Catch Errors Early**: Identify issues before they reach your repository.
- **Enforce Consistency**: Ensure all team members follow the same coding standards.
- **Save Time**: Reduce manual effort by automating repetitive tasks.

Pre-commit hooks are highly customizable and can be tailored to fit the needs of any project.

### Getting Started

#### Installation

To get started with pre-commit, you'll need to install the `pre-commit` package. You can do this using `pip`:

```bash
pip install pre-commit
```

#### Adding Pre-commit to Your Project

1. Create a `.pre-commit-config.yaml` file in the root of your project.
2. Add the hooks you want to use. Here's an example configuration:

```yaml
repos:
  - repo: https://github.com/pre-commit/pre-commit-hooks
    rev: v4.4.0
    hooks:
      - id: trailing-whitespace
      - id: end-of-file-fixer
      - id: check-yaml
      - id: check-added-large-files

  - repo: https://github.com/psf/black
    rev: 23.9.1
    hooks:
      - id: black

  - repo: https://github.com/PyCQA/flake8
    rev: 6.1.0
    hooks:
      - id: flake8
```

3. Install the hooks:

```bash
pre-commit install
```

4. Run the hooks manually on all files: 

```bash
pre-commit run --all-files
```

#### Basic Commands

- **Install hooks**: `pre-commit install`
- **Run hooks manually**: `pre-commit run`
- **Run hooks on all files**: `pre-commit run --all-files`
- **Update hooks**: `pre-commit autoupdate`

Now you're ready to use pre-commit hooks in your project! Explore the list of hooks below to find tools that fit your needs.

## 🌐Languages

- [Python](languages/Python.md)

## 🤝Contributing

We welcome contributions to **Awesome Precommit**! Whether you're submitting a new pre-commit hook, suggesting improvements, or fixing issues, your contributions are greatly appreciated. Here's how you can contribute:

### 🔧 Guidelines for Contributions

1. **New Hooks and Tools**:
   - Ensure the hook or tool is actively maintained.
   - Provide a brief description and a link to the repository.
   - Mention its primary use case (e.g., linting, formatting, security).

2. **Improvements or Fixes**:
   - Provide a clear description of the improvement or fix.
   - If you're fixing an issue, link to the relevant GitHub issue or discussion.

3. **Documentation Updates**:
   - If you notice errors or areas where documentation can be improved, feel free to suggest updates.

4. **Respect Project Structure**:
   - Follow the existing format of the list and place items under the correct category.
   - Ensure links, descriptions, and markdown formatting are consistent.

### 🛠 How to Contribute

1. **Fork the Repository**  
   Click the "Fork" button to create your own copy of the repository.

2. **Clone the Repository**  
   Clone your forked repository locally:
   ```bash
   git clone https://github.com/your-username/awesome-precommit.git
   cd awesome-precommit
```

3. **Create a New Branch**  
    Create a new branch for your feature or fix:
    
    ```bash
    git checkout -b feature-or-fix-name
    ```
    
4. **Make Changes**  
    Make your changes, and ensure you follow the guidelines.
    
5. **Test Your Changes**  
    If applicable, test your changes to ensure they work as expected.
    
6. **Commit and Push**  
    Commit your changes with a descriptive message:
    
    ```bash
    git commit -m "Add/Update [description of change]"
    git push origin feature-or-fix-name
    ```
    
7. **Submit a Pull Request**  
    Go to the original repository and submit a pull request from your branch.
    

### 🚀 Review Process

- Your pull request will be reviewed by maintainers or contributors.
- Feedback may be provided, and you may be asked to make changes.
- Once approved, your contribution will be merged into the main branch.

### 📜 Code of Conduct

Please be respectful and considerate when contributing. This project adheres to a Code of Conduct to maintain a positive and inclusive environment.

Thank you for helping improve **Awesome Precommit**!

## ⚖️License
