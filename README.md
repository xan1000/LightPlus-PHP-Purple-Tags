# Light+ PHP Purple Tags

A `color theme` for `Visual Studio Code` which includes a simple addition to the default Light+ theme to make PHP tags purple.

This extension can be found here:

https://marketplace.visualstudio.com/items?itemName=p26frqxxfmwrzekd6c6fcty5kipjkr3gaeejzpkyy42p5udjkjyq.lightplus-php-purple-tags

## Light+ PHP Purple Tags theme

![screenshot](https://raw.githubusercontent.com/xan1000/LightPlus-PHP-Purple-Tags/master/screenshots/Light%2B-PHP-Purple-Tags.png)

The issue with the default Light+ theme for PHP tags is they use the same colour as HTML tags. Thus when mixing HTML markup & PHP code it can be hard to tell them apart.

Contrast the code snippet above with the default Light+ theme.

## Light+ theme

![screenshot](https://raw.githubusercontent.com/xan1000/LightPlus-PHP-Purple-Tags/master/screenshots/Light%2B.png)

## Making PHP tags purple without this theme

You can include the rule to style PHP tags in your user settings which will then be applied to all themes.

To change the PHP syntax highlighting colors, use the following `editor.tokenColorCustomizations` in your user settings `settings.json` file:

```json
    "editor.tokenColorCustomizations": {
        "textMateRules": [
            {
                "name": "PHP Purple Tags",
                "scope": [
                    "punctuation.section.embedded.begin.php",
                    "punctuation.section.embedded.end.php"
                ],
                "settings": {
                    "foreground": "#6600CC"
                }
            },
        ]
    }
```

You can read more about themes & customisations here:

https://code.visualstudio.com/docs/getstarted/themes
