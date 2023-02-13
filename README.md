# Thoth

__Thoth__ is a GitHub repository engineered as a `plain text files` provider, hence working as a service that allows your application to read plain text files' raw content (meaning they __can not__ contain any logic) just by accessing their URL in the platform.

The main use case for this repository is to allow any product to show content that is likely to be changed over time without the hassle of neither changing the code that consumes it, nor compiling/deploying it.

> Use case example:
>
> Marketing department needs to change a commercial message before seasonal sales. Instead of hardcoding those messages into your UI, compiling the project (if that's the case) and deploying it every time that message needs to be changed, you can simply add a message in Thoth and read it from your application on demand. To update that commercial message, just change the file notifications in Thoth and you are done.

The message needs to be like the next example, you can find more information on which options you can use [here](https://docs.google.com/document/d/1cD0_p7EVUUNZ9MV1OK_Clpz4MrSBAhgiUQ5KyxR8aFY/edit#heading=h.d9wiqduhppkm): 
```json
{
  "id": "BLACK_FRIDAY_2022",
  "lang": "en",
  "products": ["addin"], 
  "licenseStatuses": ["trial"],

  // these are optional
  "startDate": "",
  "endDate": "",
  "solutions": ["word"],

  // this is optional, but if you want info in your notification, you need to write title and text
  "info": {
    "title": "BLACK WEEK MATHNESS",
    "text": "Enjoy 30% OFF for MathType Office Tools.<br/><br/><a style=\"text-decoration:underline\" href=\"https://store.wiris.com/en/individual/purchase/step1?code=BLACK22FAI&utm_source=Product&utm_medium=MathTypeMS365&utm_campaign=FancyNotification&utm_term=BlackFriday2022&utm_content=GETITNOW\" target=\"_blank\">Get 30% discount</a>"
  },

  // this is optional, but if you want to put an image, you need to write the url, the altText and the target
  "image": {
    "url":"https://assets.officetools.wiris.kitchen/gifs/black-week-sales.gif",
    "altText": "Take advantage of MathType's black week and get now a 30% off.",
    "target": "https://store.wiris.com/en/individual/purchase/step1?code=BLACK22FAI&utm_source=Product&utm_medium=MathTypeMS365&utm_campaign=FancyNotification&utm_term=BlackFriday2022&utm_content=GETITNOW"
  },

  // This is mandatory, number of times you want to show the notification to the user
  "visualizations": 3,
  // This is mandatory, it needs to be a number (more priority, greater number).
  "priority": 1,
  // This is optional, the possibilities are "error", "success", "info" and "warning"
  "alertType": ""
}
```

This project follows [Herodotos version 211105.1](https://github.com/wiris/herodotos/releases/tag/211105.1). Use the [documentation entrypoint](docs/README.md) to find out about this project.

## Who's to Blame

This project is maintained by the engineering team, thus, in order to make use of it you __must__ contact the authors in the following channel:

- [#engineering](https://wiris.slack.com/archives/C010P3E9AHH)

Feel free to leave feedback, report bugs or just come to tell how cool this project is. Moreover, this [document](docs/ISSUE_REPORTING.md) provides insights on how to report an issue.
