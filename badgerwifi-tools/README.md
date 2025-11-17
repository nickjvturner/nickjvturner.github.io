BadgerWiFi Tools
================

Changelog formatting
--------------------

The download page (`index.html`) and release history (`history.html`) both read
from `application_version.json`. Each string inside `changelog` or `comment`
arrays renders as a bullet. To create sub-bullets, indent the string with two
leading spaces per level (tabs count as two spaces). For example:

```
"changelog": [
  "Top level item",
  "  Child item",
  "    Grandchild item"
]
```

The renderer automatically nests `<ul>` lists based on that indentation.
