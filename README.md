# Template for Java application

This is a template repository for a Java application built with Gradle. This is designed to be used with the *git flow* Workflow.

## Table of contents

- [Gradle](#gradle)
- [GitHub Actions workflows](#github-actions-workflows)
- [Git Flow cheatsheet](#git-flow-cheatsheet)
  - [Initialization](#initialization)
  - [Adding a feature](#adding-a-feature)
  - [Creating a new release](#creating-a-new-release)
  - [French cheatsheet website](#french-cheatsheet-website)

## Gradle

This template includes :
- Executable jar generation
- Javadoc generation
- OS specific installers for Windows, Ubuntu and Linux with jpackage

## GitHub Actions workflows

There are two GitHub Actions workflows :
- Develop : Build and tests on push and pull request on the *develop* branch
- Release : Build, generate and publish the Javadoc on GitHub Pages, create release/pre-release with executable jar and installers when new tags are pushed

## Git Flow cheatsheet

### Initialization

To initialise the Git Flow workflow

```bash
git flow init
```
**Set the version tag prefix to "*v*"**

You should now have two branches :
- main
- develop

### Adding a feature

To start a feature
```bash
git flow feature start name_of_the_feature
```

A new branch will be created from the develop branch.

To finish the feature and merge to the develop branch
```bash
git flow feature finish name_of_the_feature
```

### Creating a new release

To start a new release
```bash
git flow release start 1.2.3
```

A new branch will be created from the develop branch with the associated tag (here with the tag 1.2.3)

To finish the release and merge it to both the develop and the main branch
```bash
git flow release finish 1.2.3
```

Then you can push the corresponding tag
```bash
git push origin --tags
```

*Before pushing the tag make sure all the local branches have been pushed*

### French cheatsheet website

https://danielkummer.github.io/git-flow-cheatsheet/index.fr_FR.html

