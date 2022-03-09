# Contributing to Thoth

## Environments and branches

Given the nature of this project, no environments exist as such. Nevertheless, three different branches have been created to make testing easier:

* development: point to this branch if you need to try changes in your developnment environment.
* staging: point to this branch when you need QA or product to test changes previosly introduced using the development branch.
* main: use this branch to references files from production environments.

For each of this environments, the URLs you should point from your code are:

| Environment | Branch       | Base URL                                                    |
|-------------|--------------|-------------------------------------------------------------|
| Develoopment| development  | <https://raw.githubusercontent.com/wiris/thoth/development> |
| Staging     | staging      | <https://raw.githubusercontent.com/wiris/thoth/staging>     |
| Production  | main         | <https://raw.githubusercontent.com/wiris/thoth/main>        |

## Conventional commits

Ideally, this project should use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), but since it's very likely that non technical collaborators commit changes to it, we can't assure this is always true. Just use them if you know what they are and make sure any other collaborators know what they mean and what they are, just in case the want to use them as well.
