# Terraform Beginner Bootcamp 2023

## Semantic Versioning :mage:

This project is going to utilize semantic versioning for its tagging. 
[semver.org](https://semver.org/)

The general format:

 **MAJOR.MINOR.PATCH**, e.g. `1.0.1`

- **MAJOR** version when you make incompatible API changes
- **MINOR** version when you add functionality in a backward compatible manner
- **PATCH** version when you make backward compatible bug fixes

## install the Terraform CLI ##

### Considerations with the Terraform CLI 
The Terraform CLI installation istructions have changed due to GPG keyring changes.
Refer to latest Terraform CLI installtion instructions.

[Install Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)

### Refactoring into Bash scripts

While fixing the Terraform CLI deprecation issues we decided to create a bash script to install the Terradorm CLI. 
-This will keeo the Gitpod task file tidy ([.gitpod.yml](.gitpod.yml)).  
-This will allow for easier debugging

https://www.cyberciti.biz/faq/how-to-check-os-version-in-linux-command-line/
https://en.wikipedia.org/wiki/Shebang_(unix)
https://en.wikipedia.org/wiki/Chmod

### Github Lifecycle (Before, Init, Command)

We need to be careful when using init because it will not rerun if we restart an existing workspace.
https://www.gitpod.io/docs/configure/workspaces/tasks