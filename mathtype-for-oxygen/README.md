# Notifications

Notifications are a special way of communication with the MathType for Oxygen users, mainly used as an extra communication channel.

## How to set a fancy notification

You can set one, and only one, notification per language. To do so, create (or modify if already present) a JSON file in this very folder with the format: `{language code}.json` where `language code` must be one of the [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) codes.

These files must contain the following JSON structure:

```json
{
  priority: [number , mandatory],
  id: [String, mandatory],
  type: [("success" | "info" | "warning" | "error") , mandatory],
  title: [String, mandatory],
  content: [String, mandatory],
  numberOfVisualizations: [number , mandatory],
}
```

## JSON fields explanation

General:

* **priority**: Mandatory number used to set the priority level of the notification. The higher the number, the higher the priority.
* **id**(*): Mandatory string used to identify any given notification. This identifier is necessary for the product internals, and must be unique.
* **type**: Notification severity level. Valid values are "success", "info", "warning", "error".
* **title**: Used as the notification title.
* **content**: Text to be shown to the user. Can be basic HTML code (bold text, italics, anchors and inline styles allowed).
* **numberOfVisualizations**: number of times the notification should be shown to the user.


(*) These values should be provided by the development team
