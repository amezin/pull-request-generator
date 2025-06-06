# Pull Request Generator Workflow

[This workflow](.github/workflows/make-pull-request.yml) creates or updates
a pull request that adds a generated file on every push to `main` branch.

1. A commit with the generated file is created

2. A branch is created or updated to point to the commit

3. A pull request is created or updated

The pull request and the branch thus always stay mergeable (fast-forward).
The branch and the pull request are reused, if possible.

It is implemented by combining together:

- https://github.com/amezin/create-commit-action

- https://github.com/amezin/create-or-update-git-ref-action

- https://github.com/amezin/create-or-update-pull-request-action
