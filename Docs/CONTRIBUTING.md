# Contributing
When contributing always follow the conventional commits

# Bramching

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
	merge your_feature tag: "v0.1.0"
	checkout main
	merge dev tag: "v0.1.0"
	commit

```

# Conventional commits
Commits messages should always be descriptive. Meaning technical descriptions without personal believes or feelings. Commits should always include any of these prefixes:

| **Prefix**   | **Use case**             |
| :------------| :------------------------| 
|`fix:`      | The commit includes fixes for existing bugs.|
features to the project.|
|`docs:`      | The commit includes documentation update.|
|`style:`     | The commit includes changes that do not affect the meaning of code.|
|`refactor:`      | A code change that neither fixes a bug nor adds a feature|
|`perf:`      | A code change that improves performance|
|`test:`      | The commit includes adding missing tests or correcting existing tests.|
|`feat:`      | The commit includes new|
|`build:`      | The commit includes changes that affect the build syste, or external dependencies.|
|`ci:`      | The commit includes changes to the Continuous Integration (CI) configuration files and scripts.|
|`chore:`      | other changes that do not modify src or test files.|
|`revert:`      | reverse a previous confirmation|

Commits should only contain changes related to the prefix used, for example: Never commit feat files with docs files.

Download the **Conventional Commit** extension for ease of use in **Visual Studio Code**

```mermaid
feat: allow provided config object to extend other configs
```
