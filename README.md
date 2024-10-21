# tinted-jqp

A Tinted Theming template for [jqp] with [Base16] and [Base24] themes.

## Usage

### Tinty

For usage with [Tinty]:

1. Add the following to `~/.config/tinted-theming/tinty/config.toml`:

   ```toml
   [[items]]
   path = "https://github.com/tinted-theming/tinted-jqp"
   name = "tinted-jqp"
   themes-dir = "themes"
   hook = "cp -f %f ~/.jqp.yaml"
   supported-systems = ["base16", "base24"]
   ```

   Note: This will overwrite any settings you have in `~/.jqp.yaml`. If
   you have existing settings make sure to combine your custom schemes
   and the themes in the `hook` property above.

2. `tinty apply base16-ayu-dark` to change the theme to
   `base16-ayu-dark`

For more information on Tinty setup or usage, have a look at the [Tinty]
GitHub page.

### Manual

Copy the contents of one of the themes in `themes/*.yaml` into your
`jqp` config file located at `~/.jqp.yaml` by default.

## Contributing

See our [Contributing] document for more information about general
template contribution.

[jqp]: https://github.com/noahgorstein/jqp
[Base16]: https://github.com/tinted-theming/home/blob/main/styling.md
[Base24]: https://github.com/tinted-theming/base24/blob/main/styling.md
[Tinty]: https://github.com/tinted-theming/tinty
[Contributing]: https://github.com/tinted-theming/home/blob/main/CONTRIBUTING_TO_TEMPLATES.md
