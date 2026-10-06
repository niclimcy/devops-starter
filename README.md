# DevOps Starter

## About

This project is a simple Python calculator created as part of a DevOps learning exercise.

## Features

The calculator supports:

- Addition
- Subtraction
- Multiplication
- Division

## How to Run

Make sure Python is installed, then run:
python calculator.py

## Author

Nicholas Lim

## Scanning

### Bandit

I used Bandit to perform static security analysis on the Python code.

During the initial scan, Bandit reported the use of assert as a low-severity security issue. After reviewing the finding, I determined that the assert statement was located in the test file and was not part of the application's production code.

Therefore, I excluded the test file from the Bandit scan to avoid reporting this known and non-production finding.

### GitHub CodeQL

In addition to Bandit, I enabled [GitHub CodeQL](https://docs.github.com/en/code-security/how-tos/find-and-fix-code-vulnerabilities/configure-code-scanning/configure-code-scanning) scanning through the Security tab of the GitHub repository.

CodeQL provides additional static analysis to identify potential security vulnerabilities and coding issues in the codebase. Using both Bandit and CodeQL provides an additional layer of security scanning as part of the development workflow.
