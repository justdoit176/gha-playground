# GitHub Actions Playground

This is designed to help experiment with and learn about GitHub Actions.

## Getting Started

To get started with GitHub Actions in this repository, follow these steps:

1. **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/gha-playground.git
    cd gha-playground
    ```

2. **Create a new workflow:**
    - Navigate to the `.github/workflows` directory.
    - Create a new YAML file for your workflow, e.g., `example-workflow.yml`.

3. **Define your workflow:**
    - Use the [GitHub Actions syntax](https://docs.github.com/en/actions/learn-github-actions/workflow-syntax-for-github-actions) to define your workflow steps.

## Example Workflow

Here is an example of a simple workflow that runs on every push:

```yaml
name: Example Workflow

on: [push]

jobs:
  build:
     runs-on: ubuntu-latest

     steps:
     - name: Checkout repository
        uses: actions/checkout@v2

     - name: Run a one-line script
        run: echo "Hello, GitHub Actions!"
```

## Resources

- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [GitHub Actions Marketplace](https://github.com/marketplace?type=actions)
