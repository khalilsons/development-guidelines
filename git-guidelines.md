## Git Guidelines


## Branches

**master** — this is where stable production ready code lands. No direct commits are allowed. Each change on this branch must be tagged with version number.

**Feature branch** - this branches off from master and merged to master by creating a PR and getting code reviews on it. naming: **username/issue_id**

## Workflow
* Feature branch is created from master
* When a feature is complete a PR is created to merge it to master.
* After code review, testing and bug fixes this branch is merged into master
* Tag the master branch to create a new release

## Commit Message

Use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) to get maximum benefit out of commit messages.


```
feat: add hat wobble

^--^ ^------------^
| |
| +-> Summary in present tense.
|
+-------> Type: chore, docs, feat, fix, refactor, style, or test.
```


More Examples:


```
chore: add Oyster build script
docs: explain hat wobble
feat: add beta sequence
fix: remove broken confirmation message
refactor: share logic between 4d3d3d3 and flarhgunnstow
style: convert tabs to spaces
test: ensure Tayne retains clothing
```

## Change Logging

A changelog is a file which contains a curated, chronologically ordered list of notable changes for each version of a project.


### Guidelines

* Changelogs are for humans, not machines.
* There should be an entry for every single version.
* The same types of changes should be grouped.
* Versions and sections should be linkable.
* The latest version comes first.
* The release date of each version is displayed.


### Types of Changes



* **Added** for new features.
* **Changed** for changes in existing functionality.
* **Deprecated** for soon-to-be removed features.
* **Removed** for now removed features.
* **Fixed** for any bug fixes.
* **Security** in case of vulnerabilities.

To reduce the effort required to maintain a changelog keep an **Unreleased** section at the top to track upcoming changes.

This serves two purposes:



* People can see what changes they might expect in upcoming releases
* At release time, you can move the Unreleased section changes into a new release version section.


## Documentation



* Use of README.md file per directory to explain the purpose of the code/items in the directory.
* REAMDE.md file of the repo parent dir to explain the repository and project.
* CONTRIBUTING.md file to outline the development and contribution method including development environment setup etc.


## Release Versioning

Given a version number MAJOR.MINOR.PATCH, increment the:

**MAJOR** version when you make incompatible changes,

**MINOR** version when you add functionality in a backwards compatible manner, and

**PATCH** version when you make backwards compatible bug fixes.

More details can be found [here](https://semver.org/) related to Semantic Versioning
