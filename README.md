# Template for Java application

This is a repository template for a Java application built with Gradle. This is designed to be used with the *git flow* Workflow.

## Gradle

This template includes :
- Executable jar generation
- Javadoc generation
- OS specific installers for Windows, Ubuntu, Linux with jpackage

## CI/CD

There are two GitHub Actions workflows :
- Develop : Build and tests on push and pull request on the *develop* branch
- Release : Build, generate and publish the Javadoc on GitHub Pages, create release/pre-release with executable jar and installers
