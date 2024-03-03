# Contributing
When contributing always follow the conventional commits

# Branching

```mermaid
gitGraph
	commit
	commit
	branch dev
	checkout dev
	commit
	commit
	branch features
	commit
	commit
	commit
	checkout dev
	merge features type: REVERSE
	checkout features
	commit
	commit
	checkout dev
	merge features tag: "v0.1.0"
	checkout main
	merge dev tag: "v0.1.0"
	commit

```

# Conventional commits
Commits messages should always be descriptive. Meaning technical descriptions without personal believes or feelings. Commits should always include any of these prefixes:

| **Prefix**   | **Use case**             |
| :------------| :------------------------| 
|`fix:`      | The commit includes fixes for existing bugs.|
|`docs:`      | The commit includes documentation update.|
|`style:`     | The commit includes changes that do not affect the meaning of code.|
|`refactor:`      | The commit include a code change that neither fixes a bug nor adds a feature.|
|`perf:`      | The commit include a code change that improves performance.|
|`test:`      | The commit includes adding missing tests or correcting existing tests.|
|`feat:`      | The commit includes new features to the project.|
|`build:`      | The commit includes changes that affect the build syste, or external dependencies.|
|`ci:`      | The commit includes changes to the Continuous Integration (CI) configuration files and scripts.|
|`chore:`      | The commit include other changes that do not modify src or test files.|
|`revert:`      | The commit include a reverse a previous confirmation.|

Commits should only contain changes related to the prefix used, for example: Never commit feat files with docs files.

Download the **Conventional Commit** extension for ease of use in **Visual Studio Code.**

Commit examples:

```bash
feat: Add user authentication feature
```

```bash
fix: Fix issue with login form validationigs
```

```bash
docs: Update installation guide
```

```bash
refactor: Simplify logic for user authentication
```

```bash
chore: Update dependencies to latest versions
```
# Issues
For issues names follow the same instructions of the [Commits](#Conventional commits) section.

Describing issues should follow the issue template for each repository

# Pull Requests
For PR names follow the same instructions of the [Commits](#Conventional commits) section.

- PR should always be created with existing Opened issues.
- PR description should point all the changes made by the devs.

PR will be always merged using `squash.`

- Make sure the description of the `Merge` contains all the commits made.