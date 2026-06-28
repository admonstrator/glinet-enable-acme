# GitHub Workflows

This directory contains automated workflows for the glinet-enable-acme project.

## Workflows

### 🧪 `test-script.yaml`
**Triggers:** Push to main/develop, Pull Requests

Comprehensive testing suite that runs on every code change:

- **ShellCheck Analysis** - Linting and best practices
- **Syntax Validation** - Tests with dash, bash, and sh
- **Flag Parsing Tests** - Validates command line arguments
- **POSIX Compliance Check** - Ensures compatibility with ash/OpenWrt
- **Log Function Tests** - Tests ASCII and emoji modes
- **README Consistency** - Verifies all flags are documented
- **Integration Checks** - Validates all functions are defined

## Local Testing

Test the script syntax locally:
```bash
sh -n enable-acme.sh
```

Run help flag test:
```bash
sh enable-acme.sh --help
```
