# Pull Request Generator Workflow

[This workflow](.github/workflows/make-pull-request.yml) creates and updates
a pull request on every push to `main` branch.

It is implemented by combining together:

- https://github.com/amezin/create-commit-action

- https://github.com/amezin/create-or-update-git-ref-action

- https://github.com/amezin/create-or-update-pull-request-action
