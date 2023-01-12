# Contributing to Thoth

## Environments and branches

Given the nature of this project, no environments exist as such. Nevertheless, three different branches have been created to make testing easier:

- development: point to this branch if you need to try changes in your development environment.
- staging: point to this branch when you need QA or product to test changes previously introduced using the development branch.
- production: point to this branch for stable, final environment calls.
- main: alias for production branch. You can use it, but is recommended to use `production` branch to keep the environment/branch naming consistency.

For each of this environments, the URLs you should point from your code are:

| Environment | Branch      | Base URL                                                    |
| ----------- | ----------- | ----------------------------------------------------------- |
| Development | development | <https://raw.githubusercontent.com/wiris/thoth/development> |
| Staging     | staging     | <https://raw.githubusercontent.com/wiris/thoth/staging>     |
| Production  | production  | <https://raw.githubusercontent.com/wiris/thoth/production>  |

## Conventional commits

Ideally, this project should use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), but since it's very likely that non technical collaborators commit changes to it, we can't assure this is always true. Just use them if you know what they are and make sure any other collaborators know what they mean and what they are, just in case the want to use them as well.
