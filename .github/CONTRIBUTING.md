# Contributing Guidelines

## Formating
- `clang-format` is used for formating
- When a PR is merged the maintainers will run it

## Comments
- Multiline comments start with a `//` at the start of the line 
- Comments should be as short as possible
- Comments should be  only over several lines if absolutely necessary
- First letter of each comment are upper case

## Branches
- Use [GitHub Flow](https://docs.github.com/en/get-started/using-github/github-flow)
- Specific and proper naming, with this convention `feature/feature-name`
- `sub-feature` branches are created by appending a `#`
- For example like this `feature/branch#sub-feature`
- All test need to pass before merging
- Debugging features are only allowed in `sub-feature` branches
- The `main` branches is protected and can only be reached via pull requests

## Commits
- Follow this [naming conventions](https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13)


## Pull Requests
- If a pull request is merged, all contributors of the pull request, must be named as [co-authors](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/creating-a-commit-with-multiple-authors)

## Refactors
- Typically made after reaching a milestone
