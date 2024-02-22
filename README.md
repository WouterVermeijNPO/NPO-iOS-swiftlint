# Introduction 
This is a repository for a shared swiftlint configuration for all NPO iOS projects.
Using this configuration we can make sure that at least the base rules are equal between all the projects.

# Getting Started
1. Add a `.swiftlint.yml` file to the project
2. Add `parent_config: https://raw.githubusercontent.com/WouterVermeijNPO/NPO-iOS-swiftlint/main/swiftlint_parent_config.yml`

Optionally, when additional rules are needed for the project, a child configuration can be added:
3. Create a `.swiftlint_refinement.yml` file
4. Add the additional rules to the child configuration file
5. Configure `.swiftlint.yml` as follows:

```yml
child_config: .swiftlint_refinement.yml
parent_config: https://raw.githubusercontent.com/WouterVermeijNPO/NPO-iOS-swiftlint/main/swiftlint_parent_config.yml
```
