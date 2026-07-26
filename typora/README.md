# Lucy for Typora

Lucy for Typora is a faithful port of the Lucy Obsidian theme. It preserves the spacious document hierarchy, full-width H1 rules, compact list rhythm, connected blockquotes, restrained Markdown markers, and separate light and dark palettes while adapting the surrounding interface to Typora.

## Install

1. In Typora, open **Settings → Appearance → Open Theme Folder**.
2. Copy these three items directly into the opened folder:
   - `lucy-light.css`
   - `lucy-dark.css`
   - the `lucy` directory
3. Restart Typora.
4. Choose **Themes → Lucy Light** or **Themes → Lucy Dark**.

Typora can assign one theme to light appearance and another to dark appearance. Select Lucy Light while the system is in light mode, select Lucy Dark while it is in dark mode, and Typora will remember both choices.

## Customize

Lucy exposes three supported customization tokens:

```css
:root {
	--lucy-accent: #7c5ce7;
	--lucy-content-width: 700px;
	--lucy-font-size: 16px;
}
```

To override Lucy Light without modifying the distributed theme, create `lucy-light.user.css` in Typora's theme folder. Use `lucy-dark.user.css` for Lucy Dark. Typora loads these files after the corresponding theme.

The light and dark themes intentionally use different default accent colors. Override `--lucy-accent` independently in each user stylesheet if you want both modes to share one accent.

## Obsidian-to-Typora equivalents

- Typora's visible Markdown metadata uses Lucy's subdued formatting-marker color.
- Typora HTML comments use Lucy's highlighted comment treatment. Typora does not parse Obsidian's `%%…%%` comment extension.
- Typora GitHub-style alerts use Lucy's callout accent.
- The title-bar document name fades in on hover or keyboard focus.
- H1 rules span the editor viewport on screen and remain inside the printable area during export.

## Development test

Open [`lucy-theme-test.md`](lucy-theme-test.md) in Typora to exercise the document elements covered by the theme. The port is developed against Typora 1.13.8 and uses current CSS features supported by modern Typora releases, including `:has()` and `color-mix()`.

