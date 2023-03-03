# Pull Requests

Did you find a bug or implemented a cool new feature? Feel free to create a Pull Request, but please adhere to the format specified below.

## Title

The title must follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) convention. It must consist of (in this order)
- a **type** (see [below](#Types)),
- an _optional_ **scope** in parentheses (see [below](#Scopes)),
- an **exclamation mark** _if and only if it is a breaking change_,
- a **colon** and a **summary** of the purpose of the Pull Request.

**Special case:** If your Pull Request only consists of a single commit, its commit message must also follow this convention. This is because in this case, GitHub uses this commit message instead of the title of the Pull Request by default as the commit message when the Pull Request is 

### Types

All types from [Commitizen](https://github.com/commitizen/conventional-commit-types/blob/master/index.json) are
allowed. Pick the one that fits best:

| Type       | Meaning                                                                   |
|------------|---------------------------------------------------------------------------|
| **`feat`** | New feature                                                               |
| **`fix`**  | Bug fix                                                                   |
| `docs`     | Documentation only changes                                                |
| `test`     | Adding missing tests or correcting existing tests                         |
| `perf`     | Changes that improve performance                                          |
| `refactor` | Changes that neither fix a bug nor add a feature                          |
| `style`    | Changes to code style (white-space, formatting, missing semi-colons, etc) |
| `build`    | Changes that affect the build system or external dependencies (e.g. npm)  |
| `ci`       | Changes to CI configuration files and scripts (e.g. GitHub Actions)       |
| `revert`   | Reverting a previous commit                                               |
| `chore`    | Other changes that don't modify src or test files                         |

### Scopes

If you want to specify exactly which part of the code is affected by your Pull Request, you can add a scope in parentheses after the [type](#Types). No specific rule applies for the choice of the scope, maybe only skim the commit history to see if a fitting scope has been used before.

### Examples

- `feat(listView): sort entries alphabetically`
- `docs: write contributing guide`
- `refactor!: drop support for older browsers` (the exclamation mark denotes a breaking change)

## Description

Use the [provided template](./PULL_REQUEST_TEMPLATE.md). It should be suggested automatically.
