# ☕ Kape for Spicetify

Kape is a warm, dark color scheme for **Spotify** via **Spicetify**, rooted in coffee, earth, and amber tones.

## Prerequisites

Before using this theme, you need to install Spicetify:

- **Linux/macOS**: Follow the [official installation guide](https://spicetify.app/docs/getting-started)
- **Windows**: Follow the [official installation guide](https://spicetify.app/docs/getting-started)

Ensure Spicetify is installed and working before proceeding.

## Installation

### Option 1: Manual Installation

1. Create the Spicetify Themes directory:
   ```bash
   mkdir -p ~/.config/spicetify/Themes/Kape
   ```

2. Copy the theme files:
   ```bash
   cp color.ini ~/.config/spicetify/Themes/Kape/
   cp user.css ~/.config/spicetify/Themes/Kape/
   ```

3. Apply the theme:
   ```bash
   spicetify config current_theme Kape
   spicetify config color_scheme Base
   spicetify apply
   ```

4. Restart Spotify to see the changes

### Option 2: Using Git (Recommended for Updates)

1. Clone this repository directly into your Spicetify themes:
   ```bash
   git clone https://github.com/kape-theme/kape-spicetify.git ~/.config/spicetify/Themes/Kape
   ```

2. Apply the theme:
   ```bash
   spicetify config current_theme Kape
   spicetify config color_scheme Base
   spicetify apply
   ```

3. To update in the future:
   ```bash
   cd ~/.config/spicetify/Themes/Kape
   git pull
   spicetify apply
   ```

## Color Palette

| Element | Hex |
|---------|-----|
| Main Background | `#181616` |
| Sidebar | `#1e1b1b` |
| Text | `#d4be98` |
| Subtext | `#bdae8b` |
| Accent | `#e7bb5c` |
| Button Hover | `#f0cc7a` |
| Selected Row | `#2e2a2a` |
| Notifications | `#7b8fd4` |
| Error Notifications | `#b53535` |

See the main [Kape repository](https://github.com/kape-theme/kape) for the complete palette with RGB and HSL values.

## Files Included

- **color.ini**: Color definitions for Spicetify
- **user.css**: Custom CSS styling

## Customization

To customize the theme, edit the files in `~/.config/spicetify/Themes/Kape/`:

1. **color.ini**: Change color hex values
2. **user.css**: Modify CSS styles

After editing, reapply:
```bash
spicetify apply
```

## Troubleshooting

- **Theme not showing**: Make sure the theme folder name exactly matches the `current_theme` value
- **Colors not applying**: Run `spicetify restore` then `spicetify apply`
- **Spotify crashes**: Revert to default theme: `spicetify config current_theme Default && spicetify apply`
- **Changes not appearing**: Clear browser cache in Spotify and restart

## Contributing

Found an issue or have a suggestion? Open an issue or PR on the [main Kape repository](https://github.com/kape-theme/kape).

## License

MIT © gabiuz
