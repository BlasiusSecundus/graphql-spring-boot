Table of Contents
=================

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [Contributing to the GraphQL Spring Boot project](#contributing-to-the-graphql-spring-boot-project)
  - [Welcome to the project](#welcome-to-the-project)
  - [Commit messages](#commit-messages)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

Contributing to the GraphQL Spring Boot project
===============================================

Welcome to the project
-----------------------

Contributions are welcome. Please respect the [Code of Conduct](http://contributor-covenant.org/version/1/3/0/) and
 the [Contribution Guideline](https://opensource.guide/how-to-contribute/#how-to-submit-a-contribution).

Commit messages
---------------

This project uses the [Conventional Commits](https://www.conventionalcommits.org) specification for commit messages.
The CI pipeline validates that commit messages adhere to the specification using 
[commitlint](https://github.com/conventional-changelog/commitlint).

**Note**: *Historical commits, made before applying this convention may not fulfill the requirements of the 
specification. These commits are exempt from this check.*

To check commit messages before committing, go to the `commitlint` folder and run `npm ci && npm run add-commitlint-git-hook` 
(you will need NodeJS installed on your machine). This command sets up a git hook to run commitlint before each commit,
to prevent committing with invalid commit messages in the first place.

**Note**: *Please always use `npm ci` instead of `install` to prevent unwanted changes to `package-lock.json`.*

To remove the git hook, just delete the `commitlint/.husky` folder.

As for the optional scope part of the commit message:
- if your commit addresses an issue, please refer the issue number in the scope - e.g. `fix(#123): ...`
- otherwise, if applicable, please use the modified / affected subproject name, without the repetitive prefix/postfix 
  parts (like `graphql-kickstart-spring-boot`, `spring-boot-starter` or `autoconfigure`) - e.g. `feat(webflux): ...`  

