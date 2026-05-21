# Nulltone

Nulltone is a display-first VS Code color theme by `oosuhada`, designed to maximize clarity, contrast, and usable screen space on Mini LED, OLED, and MacBook displays.

The name combines `null` and `tone`: not a lack of color, but a more deliberate kind of restraint. Nulltone is built around neutral values, clean contrast, and minimal accents for long coding sessions where blue-gray dark themes can feel hazy, cramped, or visually heavy.

Marketplace ID: `oosuhada.nulltone`

## Preview

<p align="center">
  <img src="./assets/nulltone-dark-preview.png" alt="OS Nulltone Dark preview" width="49%" />
  <img src="./assets/nulltone-light-preview.png" alt="OS Nulltone Light preview" width="49%" />
</p>

- **OS Nulltone Dark**: optimized for Mini LED and OLED displays with neutral black surfaces, clear white text, refined gray comments, and focused VS Code blue accents.
- **OS Nulltone Light**: optimized for bright environments and MacBook displays with clean white surfaces, readable dark text, and stronger token contrast.

## Why Nulltone

Many dark coding themes use blue-gray surfaces. On Mini LED and OLED displays, those colors can make black areas look less crisp and reduce the sense of depth that these panels are capable of.

Nulltone takes a different approach. It keeps the base palette close to neutral black, gray, and white, then uses color only where it improves meaning: syntax, focus, selection, Git state, diagnostics, and primary UI actions.

The goal is not to make the editor colorful. The goal is to make the screen feel cleaner, sharper, and easier to read for long programming sessions.

## Themes

### OS Nulltone Dark

A dark theme for high-contrast modern displays.

- Neutral black surfaces without a blue-gray cast.
- Bright foreground text where the editor should actually read as white.
- Refined gray comments instead of classic green comments.
- VS Code blue for cursor, focus, selection, badges, and primary UI accents.
- Designed to feel crisp on Mini LED, OLED, and MacBook screens.

### OS Nulltone Light

A light theme for bright rooms, classrooms, and daytime coding.

- Clear white surfaces.
- Stronger syntax contrast than many soft light themes.
- Controlled accent colors that remain readable on bright backgrounds.
- Designed for users who switch between dark and light mode throughout the day.

## Design Philosophy

Nulltone starts from achromatic space, but it is not colorless. Its color is edited down.

Most dark coding themes lean into blue-gray surfaces. On Mini LED and OLED displays, that can make the editor feel less black, less crisp, and visually heavier than intended. OS Nulltone Dark keeps the base palette between black and white without a blue cast, then reserves color for meaning: focus, selection, syntax, Git state, diagnostics, and UI accents.

The main accent follows the familiar VS Code blue family. It should feel native to the editor rather than decorative. Comments avoid the classic green retro look and use neutral gray instead, so code keeps a modern, technical tone.

OS Nulltone Light follows the same logic from the other side: white surfaces, dark readable text, and token colors with enough weight to survive real daylight and high-brightness screens.

## Palette Intent

- Neutral black and gray surfaces, without blue-gray bias.
- Bright foreground text where the editor should actually read as white.
- Refined gray comments instead of green comments.
- VS Code blue for cursor, focus, selection, badges, and primary UI accents.
- Saturated but controlled token colors for readability in light mode.
- High clarity on Mini LED, OLED, and MacBook displays.

## Recommended Usage

For the best experience, enable automatic system color mode detection in VS Code:

```jsonc
{
  "window.autoDetectColorScheme": true,
  "workbench.preferredDarkColorTheme": "OS Nulltone Dark",
  "workbench.preferredLightColorTheme": "OS Nulltone Light"
}
```

This lets VS Code follow macOS light and dark mode automatically.

## Future Variants

Nulltone is designed as a family:

- `OS Nulltone Dark`
- `OS Nulltone Light`
- `OS Nulltone Amber`
- `OS Nulltone Mono`

## Local Development

Open this folder in VS Code and run the extension development host:

1. Press `F5`.
2. Choose **OS Nulltone Dark** or **OS Nulltone Light** from the Color Theme picker.

The `reference/` directory is intentionally ignored by Git. It contains local study material from other open-source VS Code themes and is not packaged with Nulltone.
