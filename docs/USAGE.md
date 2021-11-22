# Using Thoth

Thoth acts as a `plain text repository` hosted by Github. If you application needs to consume a file content with no logic involved, Thoth can help you.

To do so, follow the next steps:

  1. Create a folder with a significative name in the root directory of the project (if it does not exist yet). No rules regarding naming folder have been set yet, so just use the common sense.
  2. Create as many `plain text files` as needed in that folder. How you name those files is up to you. Again, apply the common sense.
  3. Go to the repository [page in GitHub](https://github.com/wiris/thoth), browse to the file you need to consume from your application, and open it as "raw". This way, GitHub will show you it's content in a new tab.
  4. Copy that tab's URL: that's the one your code should use to consume the file content.

## How to add, modify, or remove files

You can use GitHub itself to perform any of these actions. Anyway, if you feel comfortable with Git, you should do any of these actions just be pulling and pushing the necessary commits.

## About code review

TODO: Define PR policies.

## Some security concerns

Since Thoth is a private project, nobody outside Wiris organization should be able to modify the files in the repository. Anyways, is a good practice to sanitize the content of the files you consume from Thoth, just in case.
