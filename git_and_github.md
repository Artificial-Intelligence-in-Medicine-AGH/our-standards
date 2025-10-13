# Git and Github

All development is version-controlled using Git. We keep our repositories on GitHub.

## Workflow

Every project may have it's own workflow details, but as a baseline, the recommended approach is to use Feature Branches (read more [HERE](https://git-scm.com/book/en/v2/Git-Branching-Branching-Workflows)):

- Have the stable branch named `main` or `master`
- Have a development branch named `dev` - it may be unstable
- Create separate feature branch for each change (i.e.: new feature, bug fix, etc)

The feature branch should be created from `dev`, and after the change is implemented, the branch should be merged into `dev`.

`dev` can be merged into `main` branch after proper testing to ensure stability.

**No hotfixes**!

Merges should be done using Pull Requests, with at least one code review, by a person who did NOT write the change.

Feature branch should be **deleted** after being merged.

## Issues

GitHub issues should be used to specify what yet needs to be done in the project. They should be created for any bug that has been found, and new feature proposals. The feature branch should always be created in relation to one issue: i.e. one issue is resolved by one feature branch, which is merged in one Pull Request.

## .gitignore

Things that should NEVER enter git:

- python virtual environment
- .`idea` folder (created by PyCharm)
- `__pycache__` folder
- `.env` file