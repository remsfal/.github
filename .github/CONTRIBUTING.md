# Remsfal Backend

Remsfal Backend is an open-source backend service for managing and serving data for the Remsfal project. This project is part of an university curriculum and is being partly developed by a group of students.

## Building and Working with the Codebase

For instructions on how to build and work with the Remsfal backend codebase, please refer to the [Building Guide](https://github.com/remsfal/remsfal-backend/blob/main/README.md).

## Contributing to Remsfal Backend

Remsfal Backend is a community-driven project, and we welcome contributions and feedback. To help streamline contributions, please review the following guidelines to ensure a smooth process.

If you plan to contribute a larger change, we recommend starting with a discussion. This helps identify if the proposed change aligns with the project’s goals and provides an opportunity for early feedback. For smaller changes, feel free to directly submit a pull request.

Here’s a quick checklist for a good PR (details provided below):

1. Start with a discussion for major changes.
2. Open a GitHub Issue with a detailed description, linked to your PR.
3. One feature/change per PR.
4. One commit per PR.
5. Rebase on the `main` branch (`git rebase`, not `git pull`).
6. Write a clear commit message with a link to the issue.
7. Keep changes focused on the intended functionality.
8. Include functional and integration tests.
9. Update documentation where necessary.

Once submitted, please monitor your PR for any feedback. Note that we may close inactive PRs after two weeks of no response. You are welcome to reopen or submit a new PR if it is closed due to inactivity.

### Finding Issues to Work On

If you’d like to contribute but aren’t sure where to start, take a look at [open issues](https://github.com/remsfal/remsfal-backend/issues). These include various tasks, from simple to complex, that need contributions.

### Starting a Discussion for Proposed Changes

For major changes, please open a [GitHub Discussion](https://github.com/remsfal/remsfal-backend/discussions). This is where we can discuss the proposed idea and gather feedback. You may also use our community mailing list if needed for more in-depth technical discussions.

### Creating an Issue

When opening an issue, please provide a clear summary and detailed description. This will help reviewers understand your proposed changes and will serve as a reference for the community in the future.

### Creating a Branch to Work On

When working on a new feature or bug fix, create a new branch from the `main` branch. This helps keep your changes isolated and makes it easier to merge them back into the main codebase.

The format for branch names should be `issue-<issue-number>-short-description`. For example, `issue-#1234-fix-typo`.

Tip: To change the name of a branch you’re currently on, use `git branch -m <new-branch-name>`. If you’re on a different branch, use `git branch -m <old-branch-name> <new-branch-name>`.

### Implementing Changes

Instructions for building the project from source and general guidelines for contributing can be found in the [Building Guide](https://github.com/remsfal/remsfal-backend/blob/main/README.md).

Please avoid formatting or refactoring code unrelated to your change, as this increases review complexity. If code refactoring is necessary, submit it as a separate PR.

### Writing Tests
When making code changes, please ensure to include both functional tests and integration tests. This helps validate your changes and prevents potential regressions. For help with writing tests, reach out to our community.

To ensure comprehensive test coverage, consider the following:

* Write functional tests to isolate and test each function, class, or module. This checks the correctness of small code units and ensures each performs its intended functionality.
* Write integration tests to check that different parts of your code work together correctly. This can involve checking the behaviour of your code in the context of the entire system or in interaction with external systems.
* Add tests for both the success and failure paths of your code.
* Try to write tests that can predict the behaviour of your code under different conditions or with different inputs.

Remember to check your tests locally before opening a PR. This helps keep our CI free for running tests on open PRs and speeds up the review process.

### Documentation

Make sure to include any relevant documentation updates with your code changes. Review this Documentation and other [Current Documentation's](https://github.com/remsfal/remsfal-backend/blob/main/README.md) to ensure consistency.

### Submitting a Pull Request (PR)

When submitting your PR, ensure:

1. The branch is rebased on the latest `main` branch.
2. Your PR has a single, well-structured commit.
3. The commit message clearly describes the change and includes a link to the issue.

To rebase, use `git rebase` instead of `git pull`. This approach keeps the commit history clean and improves the review process. For help with rebasing, check out the [Git Documentation](https://git-scm.com/book/en/v2/Git-Branching-Rebasing).

### Developer's Certificate of Origin

Please make sure your contributions can legally be included in the Remsfal project, and sign off your commits with `--signoff` or `-s` to indicate your agreement to the [Developer’s Certificate of Origin](https://developercertificate.org/)

### Commit messages and issue linking

The format for a commit message should look like:

```
A brief descriptive summary

Optionally, more details around how it was implemented

Closes #1234
``` 

The very last part of the commit message should be a link to the GitHub issue, when done correctly GitHub will automatically link the issue with the PR. There are 3 alternatives provided by GitHub here:

* Closes: Issues in the same repository
* Fixes: Issues in a different repository (this shouldn't be used, as issues should be created in the correct repository instead)
* Resolves: When multiple issues are resolved (this should be avoided)

Although, GitHub allows alternatives (close, closed, fix, fixed), please only use the above formats.

Creating multi line commit messages with `git` can be done with:

```
git commit -s -m "Summary" -m "Optional description" -m "Closes #1234"
```

Alternatively, `shift + enter` can be used to add line breaks:

```
$ git commit -s -m "Summary
> 
> Optional description
> 
> Closes #1234"
```

For more information linking PRs to issues refer to the [GitHub Documentation](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue).


