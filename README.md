# Obsidian for Zed

A Zed port of Fernando Jiménez's Obsidian 3.0.0 theme for the IntelliJ Platform.
It includes both original variants:

- `Obsidian` (dark)
- `Obsidian Bright` (light)

The UI colors were translated from the IntelliJ theme JSON files, while editor,
syntax, search, diff, and terminal colors were translated from the IntelliJ color
schemes. IntelliJ-only concepts were mapped to the closest Zed semantic roles.

## Install as a development extension

1. Open Zed's command palette.
2. Run `zed: extensions`.
3. Select **Install Dev Extension**.
4. Choose this directory (`Obsidian-Zed`), not the `themes` subdirectory.
5. Open the theme selector and choose `Obsidian` or `Obsidian Bright`.

For automatic light/dark switching, use these names in Zed's settings:

```json
{
  "theme": {
    "mode": "system",
    "dark": "Obsidian",
    "light": "Obsidian Bright"
  }
}
```

The original IntelliJ schemes specify Fira Code at 15 px, ligatures enabled, and
1.4 line spacing. Zed themes cannot set font preferences, so configure those in
your Zed settings separately if you want the closest match.

## Local-theme alternative

Copy `themes/obsidian.json` to `%USERPROFILE%\AppData\Roaming\Zed\themes\` and
reload Zed. This does not require installing the directory as an extension.

## Port notes

- Theme schema: Zed `v0.2.0`
- Source: IntelliJ Obsidian plugin `3.0.0`
- Verified with the installed Zed CLI version `1.19.2`
- Original theme repository: <https://github.com/luisfer0793/theme-obsidian>
