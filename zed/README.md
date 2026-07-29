# Lucy for Zed

Lucy for Zed is a light/dark editor theme that carries Lucy's restrained
palette into Zed's application chrome, editor, syntax highlighting, terminal,
Git states, diagnostics, and collaboration cursors.

Zed themes do not control rendered Markdown layout, font sizes, line height, or
document width. Those parts of the Obsidian and Typora experience therefore
remain editor settings rather than theme behavior.

## Installation

1. Download and extract `lucy-zed.zip`, or use this directory from the
   repository.
2. Open Zed's local themes directory:
   - macOS and Linux: `~/.config/zed/themes`
   - Windows: `%USERPROFILE%\AppData\Roaming\Zed\themes\`
3. Copy `lucy.json` into that directory. Create the `themes` directory if it
   does not exist.
4. Reload Zed.
5. Open the theme selector with `cmd-k cmd-t` on macOS or `ctrl-k ctrl-t` on
   Linux and Windows, then choose **Lucy Light** or **Lucy Dark**.

## Automatic light/dark pairing

Add this object to Zed's `settings.json` to follow the system appearance:

```json
{
  "theme": {
    "mode": "system",
    "light": "Lucy Light",
    "dark": "Lucy Dark"
  }
}
```

The following optional settings are close to Lucy's compact, readable defaults.
They are settings rather than theme properties, so the theme intentionally does
not modify them:

```json
{
  "ui_font_size": 14,
  "buffer_font_family": ".ZedMono",
  "buffer_font_size": 15
}
```

## Scope

The package includes:

- Lucy Light and Lucy Dark in one Zed theme family;
- Lucy's purple light accent and steel-blue dark accent;
- application surfaces, panels, tabs, dialogs, scrollbars, and focus states;
- editor selections, guides, invisibles, search matches, and Markdown titles;
- restrained syntax colors for code and markup;
- terminal ANSI colors, diagnostics, Git states, and collaboration cursors.

The package does not imitate Obsidian or Typora controls inside Zed. It uses
Zed's native theme interface and preserves the editor's behavior.
