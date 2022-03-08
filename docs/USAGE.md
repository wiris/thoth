# Using Thoth

Thoth acts as a `plain text repository` hosted by Github. If your application needs to consume a file content with no logic involved, Thoth can help you.

## Before using Thoth

First off: before you use Thoth, you must contact the [engineering team](https://wiris.slack.com/archives/C010P3E9AHH) to approve its use and then read the [contributing guidelines](./CONTRIBUTING.md) and make sure you understand them.

Besides that, you must take into account some of Thoth's limitations:
  
  1. This project acts as basic `plan text file` server. __No logic can be involved in those files__. Furthermore, no logic __should be__ involved in the use of this service.
  2. Thoth has been set as a __public GitHub repository__ to work as intended, meaning __no confidential, compromising data can be included in it__.
  3. GitHub allows a maximum of 5000 requests/hour for raw files (more info about this in the  [official GitHub documentation](https://docs.github.com/en/rest/overview/resources-in-the-rest-api#rate-limiting)).

  > We are not really sure that GitHub limitation really affects us, let's keep it in mind, just in case.

## I contacted the engineering team and understand the limitations

Once the engineering team approve the use of Thoth, and having taken into consideration its limitations, you can follow the next steps:

  1. Create a directory with a meaningful name in the root directory of the project (if it does not exist yet). No rules regarding naming directory have been set yet, so just use the common sense.
  2. Create as many `plain text files` as needed in that directory. How you name those files is up to you. Again, apply the common sense.
  3. Go to the repository [page in GitHub](https://github.com/wiris/thoth), browse to the file you need to consume from your application, and open it as "raw". This way, GitHub will show you it's content in a new tab.
  4. Copy that tab's URL: that's the one your code should use to consume the file content.

## How to add, modify, or remove files

You can use GitHub itself to perform any of these actions. Anyway, if you feel comfortable with Git, you should do any of these actions just be pulling and pushing the necessary commits.

## About code review

If you are modifying already existent files, a PR involving your squad is enough.

On the other side, if a new product is to be included in Thoth, is mandatory to include the engineering leads in the code review.

## Some security concerns

Since Thoth is a private project, nobody outside Wiris organization should be able to modify the files in the repository. Anyways, is a good practice to sanitize the content of the files you consume from Thoth, just in case.
