# Thoth

__Thoth__ is a GitHub repository engineered as a `plain text files` provider, hence working as a service that allows your application to read plain text files' raw content (meaning they __can not__ contain any logic) just by accessing their URL in the platform.

The main use case for this repository is to allow any product to show content that is likely to be changed over time without the hassel of neither changing the code that consumes it, nor compiling/deploying it.

> Use case example:
>
> Marketing department needs to change a commercial message before seasonal sales. Instead of hardcoding those messages into your UI, compiling the project (if that's the case) and deploying it everytime that message needs to be changed, you can simply add a file in Thoth and read it from your application on demand. To update that commercial message, just change the file in Thoth and you are done.

This project follows [Herodoto version 211105.1](https://github.com/wiris/herodotos/releases/tag/211105.1). Use the [documentation entrypoint](docs/README.md) to find out about this project.

## Who's to Blame

This project is mantained by the engineering team, thus, in order to make use of it you __must__ contact the authors in the following channel:

- [#engineering](https://wiris.slack.com/archives/C010P3E9AHH)

Feel free to leave feedback, report bugs or just come to tell how cool this project is. Moreover, this [document](docs/ISSUE_REPORTING.md) provides insights on how to report an issue.
