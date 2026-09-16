# Contributing

Thank you for contributing to this project. Contributions from both organization members and the broader community are welcome.

Please read this document before opening an issue or pull request. By contributing, you agree to follow our code of conduct and the contribution requirements below.

## Before You Start

Before contributing:

1. Read the repository's `README.md` and relevant documentation.
2. Check existing issues and pull requests for related work.
3. For substantial changes, open an issue describing the problem and proposed solution before implementing it.
4. Make sure your changes are consistent with the project's existing architecture and conventions.
5. Ensure that you are permitted to contribute the code, documentation, or other material you submit.

## Contribution Workflow

We use different contribution workflows depending on whether you are a member of the organization.

### Organization Members

Organization members should work through branches in the canonical repository.

The general workflow is:

```text
main
  └── <user>/<type>/<short-description>
        └── Pull Request → main
```

1. Start from an up-to-date `main` branch.
2. Create a descriptive branch in the canonical repository.
3. Make your changes on that branch.
4. Push the branch to the canonical repository.
5. Open a pull request against `main`.
6. Address review feedback.
7. Once approved and required checks pass, the branch may be merged according to repository permissions and project policy.
8. Delete the branch after it is no longer needed.

Do not commit directly to `main` unless the repository explicitly permits it for a particular administrative or emergency task.

#### Branch Naming

Use a descriptive prefix where practical:

- `feature/<description>`
- `fix/<description>`
- `docs/<description>`
- `refactor/<description>`
- `test/<description>`
- `chore/<description>`

Keep branch names short, descriptive, and lowercase where possible.

### Non-Members

Contributors who are not members of the organization should use the fork-based workflow.

The general workflow is:

```text
Canonical repository
        │
        └── Fork
             │
             └── feature/<short-description>
                    │
                    └── Pull Request → canonical repository/main
```

1. Fork the repository.
2. Clone your fork locally.
3. Add the canonical repository as an upstream remote.
4. Create a branch from the current `upstream/main`.
5. Make your changes on that branch.
6. Add or update tests as appropriate.
7. Run formatting, linting, tests, and other required checks.
8. Push the branch to your fork.
9. Open a pull request from your fork to the canonical repository's `main` branch.
10. Address review feedback and keep your branch synchronized with `upstream/main` when necessary.
11. Once approved and required checks pass, a maintainer may merge the pull request.

For example:

```bash
git clone https://github.com/YOUR-USERNAME/PROJECT.git
cd PROJECT

git remote add upstream https://github.com/ORGANIZATION/PROJECT.git

git fetch upstream
git checkout -b feature/my-change upstream/main

# Make changes...

git push -u origin feature/my-change
```

Do not open pull requests from `main` in your fork for feature work. Using a dedicated branch makes it easier to update, review, and maintain your contribution.

## Pull Requests

A good pull request should:

- Have a clear, descriptive title.
- Explain what changed and why.
- Reference relevant issues when applicable.
- Include tests for new or changed behavior where appropriate.
- Update documentation when behavior or public interfaces change.
- Keep unrelated changes out of the PR.
- Pass all required automated checks.
- Be reasonably scoped so that it can be reviewed effectively.

### Pull Request Checklist

Before submitting a pull request, verify:

- [ ] The change is related to an existing issue or has an appropriate explanation.
- [ ] The code follows project conventions.
- [ ] Tests have been added or updated where appropriate.
- [ ] Existing tests pass.
- [ ] Formatting and linting pass.
- [ ] Documentation has been updated where necessary.
- [ ] No secrets, credentials, or private information have been committed.
- [ ] The diff contains only relevant changes.
- [ ] Commit history is reasonably clean and understandable.

## Testing

Contributors are expected to test their changes appropriately.

## Review Process

Pull requests are reviewed for correctness, maintainability, scope, compatibility, and adherence to project conventions.

Reviewers may request changes before a pull request is merged. Contributors are expected to respond to review comments and update their branch as necessary.

Passing CI does not guarantee that a pull request will be merged. Automated checks and human review serve different purposes.

Maintainers may also request that a change be split into smaller pull requests when doing so makes review and maintenance easier.

## Code of Conduct

All contributors are expected to participate respectfully and constructively.

Please follow the project's `CODE_OF_CONDUCT.md` where one exists. Maintainers may moderate contributions, discussions, and other project spaces to maintain a productive environment.

## License

By contributing, you agree that your contributions may be distributed under the license applicable to this project, subject to the terms described in the repository's `LICENSE` file and any applicable contributor or organizational agreements.

If you are unsure whether you have the right to submit particular material, do not submit it until the licensing situation has been clarified.

## Questions

If you are unsure how to contribute, open a discussion or issue using the project's normal communication channels.

For organization members, use the organization's internal development channels where appropriate.

Thank you for helping improve the project.