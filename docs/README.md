# Thoth

__Thoth__ is a GitHub repository engineered as a `plain text files` provider, hence working as a service that allows your application to read plain text files raw content (meaning they __can not__ contain any logic) just by accessing their URL in the platform.

The main use case for this repository is to allow any product to show content that is likely to be changed over time without the hassel of neither changing the code that consumes it, nor compiling/deploying it.

> Use case example:
>
> Marketing department needs to change a comomercial message before seasonal sales. Instead of hardcoding those messages into your UI, compiling the project (if that's the case) and deploying it everytime that message needs to be changed, you can simply add a file in Thoth and read if from you application on demand. To update that commercial message, just change the file in Thoth and you are done.

The structure of the project is described [here](./STRUCTURE.md).

## How to Use the Project

To know how Thoth can help you, please read [this document](./USAGE.md).
