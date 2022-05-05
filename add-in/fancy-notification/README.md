# Fancy notifications

Fancy notifications are a special way of communication with the MathType add-in for Microsoft Office users, mainly used to explain some concepts with the help of animated images.

## How to set a fancy notification

You can set one, and only one, fancy notification per language. To do so, create (or modify if already present) a JSON file in this very folder with the format: `{language code}.json` where `language code` must be one of the [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) codes.

These files must contain the following JSON structure:

```json
{
  "id": [String, mandatory],
  "info": {
    "title": [String, optional]
  },
  "image" [Object, optional]: {
    "url": [URL, mandatory],
    "altText": [String, mandatory],
    "target": [URL, optional]
  },
  "text": [String, optional]
}
```

## JSON fields explanation

General:

* **id**(*): Mandatory string used to identify any given fancy notification. This identifier is necessary for the add-on internals, and must be different unique.
* **info.title**: Optional string. If present, will be used as the alert title.

Image:

* **image.url**(*): Mandatory URL. Points to the animated image (i.e.: the GIF file) to be shown.
* **image.altText**: Mandatory string. Used as text to be spoken by screen readers when they come across the animated image.
* **image.target**: Optional URL. If present, clicking the notification will open an internet browser tab pointing to this URL.

Body:

* **text**: text to be shown to the user. Can be basic HTML code (bold text, italics, anchors and inline styles allowed).

(*) These values should be provided by the development team
