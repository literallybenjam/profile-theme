# PROFILE

A CSS website theme for profile pages and blogs

## BASIC PAGE LAYOUT

To use the PROFILE theme, you should structure your page according to the following layout:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
        <meta charset="utf-8">
        <link rel="stylesheet" type="text/css" href="theme.css">
    </head>
    <body>
        <header>
            <img alt="Profile Image" src="profile_image.png">
            <h1><a href="/">Page Title</a></h1>
            <hr>
            <!--  page description / profile info / etc.  -->
        </header>
        <main>
            <!--  page content  -->
        </main>
    </body>
</html>
```

You can include other children of the `<body>` element if you want, but there should be exactly one `<header>` child.

## PROFILE IMAGE

The profile image selected by `header > img` is, by default, circular. If you prefer a rectangular shape, you can select this by setting the `data-shape` attribute to `"rectangle"` on the `<img>` element.

## COLOURS

You can change the colour of an element by using the `data-colour` attribute (note `data-color` is not currently supported). The following colour-names are available:

`cyan` `blue` `purple` `magenta` `red` `yellow` `green` `teal`

Leaving the `data-colour` attribute blank will produce a neutral grey. Additionally, the colour-name may be prefixed or suffexed with `-light` or `-dark` to lighten or darken the colour; on their own, `light` produces a near-white and `dark` produces a dark grey.

`data-colour` might not act predictably when nested.
