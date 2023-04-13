# Contributing

Your contributions to this project are very welcome, be it a new feature, a bugfix, better documentation, or something else. Feel free to create a pull request, but please adhere to the [format](#format-of-a-pull-request) specified below. This strict format is required so [`semantic-release`](https://github.com/semantic-release/semantic-release) can automatically handle [semantic versioning](https://semver.org/) and update changelogs. An automated check ensures that pull requests have a matching title:

![image](https://user-images.githubusercontent.com/2501322/231755824-23cf987d-bf1b-4782-be23-89fc3d0f95ae.png)

If this check fails, simply edit the title of the pull request. There is no need to close it and to create a new one.

## Format of a Pull Request

### Title

The title must follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) convention. It must consist of (in this order)
- a **type** (see [below](#Types)),
- an _optional_ **scope** in parentheses (see [below](#Scopes)),
- an **exclamation mark** _if and only if it is a breaking change_,
- a **colon** and a **summary** of the purpose of the pull request.

#### Types

All types from [Commitizen](https://github.com/commitizen/conventional-commit-types/blob/master/index.json) are
allowed. Pick the one that fits best:

| Type       | Meaning                                                                  |
|------------|--------------------------------------------------------------------------|
| **`feat`** | New feature                                                              |
| **`fix`**  | Bug fix                                                                  |
| `docs`     | Documentation only changes                                               |
| `test`     | Adding missing tests or correcting existing tests                        |
| `perf`     | Changes that improve performance                                         |
| `refactor` | Changes that neither fix a bug nor add a feature                         |
| `style`    | Changes to code style (whitespace, formatting, missing semicolons, etc)  |
| `build`    | Changes that affect the build system or external dependencies (e.g. npm) |
| `ci`       | Changes to CI configuration files and scripts (e.g. GitHub Actions)      |
| `revert`   | Reverting a previous commit                                              |
| `chore`    | Other changes that don't modify src or test files                        |

#### Scopes

If you want to specify exactly which part of the code is affected by your pull request, you can add a scope in parentheses after the [type](#Types). No specific rule applies for the choice of the scope, just skim the commit history to see if a fitting scope has been used before.

#### Examples

- `feat(listView): sort entries alphabetically`
- `docs: write contributing guide`
- `refactor!: drop support for older browsers` (the exclamation mark denotes a breaking change)

### Description

Use the [provided template](./PULL_REQUEST_TEMPLATE.md). It should be suggested automatically.
