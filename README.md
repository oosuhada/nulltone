# Nulltone

Nulltone is a display-first VS Code color theme by `oosuhada`, designed to maximize clarity, contrast, and usable screen space on Mini LED, OLED, and MacBook displays.

The name combines `null` and `tone`: not a lack of color, but a more deliberate kind of restraint. Nulltone is built around neutral values, clean contrast, and minimal accents for long coding sessions where blue-gray dark themes can feel hazy, cramped, or visually heavy.

Marketplace ID: `oosuhada.nulltone`

## 한국어 요약

Nulltone은 Mini LED·OLED·MacBook 디스플레이에서 장시간 코딩할 때 **중립적인 명암, 선명한 대비, 최소한의 포인트 컬러**를 유지하도록 설계한 VS Code 테마입니다. 흔한 청회색 계열 dark theme 대신 실제 검정에 가까운 surface와 읽기 쉬운 회색/흰색 계층을 사용하고, 색상은 syntax·focus·selection·Git·diagnostic처럼 의미가 필요한 곳에만 남깁니다.

- **Dark / Light / Glass Dark / Glass Light** 변형 제공
- Mini LED와 OLED에서 black level과 가독성을 살리는 display-first 설계
- VS Code 기본 UI와 어색하게 충돌하지 않는 절제된 accent
- 실제 코드 화면을 기준으로 한 dark/light preview 포함
- Marketplace ID: `oosuhada.nulltone`

이 프로젝트는 단순 색상 취향 저장소가 아니라, 디스플레이 특성과 장시간 개발 환경을 고려해 하나의 작은 개발자 도구 제품으로 정리한 작업입니다.

## Preview

<p align="center">
  <img src="./assets/nulltone-dark-preview.png" alt="OS Nulltone Dark preview" width="49%" />
  <img src="./assets/nulltone-light-preview.png" alt="OS Nulltone Light preview" width="49%" />
</p>

- **OS Nulltone Dark**: optimized for Mini LED and OLED displays with neutral black surfaces, clear white text, refined gray comments, and focused VS Code blue accents.
- **OS Nulltone Light**: optimized for bright environments and MacBook displays with clean white surfaces, readable dark text, and stronger token contrast.
- **OS Nulltone Glass Dark**: a neutral transparent dark variant for the Nulltone Glass Controller. Code and terminal surfaces remain more opaque than surrounding UI.
- **OS Nulltone Glass Light**: a neutral transparent light variant for automatic macOS light mode when Glass is enabled.

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

### OS Nulltone Glass Dark / Light

Transparent variants for local use with the Nulltone Glass Controller.

- Keep the Nulltone achromatic base instead of blue-gray surfaces.
- Preserve automatic macOS dark/light switching through VS Code preferred themes.
- Use alpha only on structural surfaces, not token colors.
- Keep editor and terminal backgrounds more opaque than sidebars, tabs, and panels.
- Reserve VS Code blue for focus, cursor, selection, badges, and primary UI accents.

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

For the local glass setup:

```jsonc
{
  "window.autoDetectColorScheme": true,
  "workbench.preferredDarkColorTheme": "OS Nulltone Glass Dark",
  "workbench.preferredLightColorTheme": "OS Nulltone Glass Light"
}
```

The normal Nulltone themes remain the safe fallback when Glass is off.

## Future Variants

Nulltone is designed as a family:

- `OS Nulltone Dark`
- `OS Nulltone Glass Dark`
- `OS Nulltone Light`
- `OS Nulltone Glass Light`
- `OS Nulltone Amber`
- `OS Nulltone Mono`

## Local Development

Open this folder in VS Code and run the extension development host:

1. Press `F5`.
2. Choose **OS Nulltone Dark**, **OS Nulltone Light**, **OS Nulltone Glass Dark**, or **OS Nulltone Glass Light** from the Color Theme picker.

The `reference/` directory is intentionally ignored by Git. It contains local study material from other open-source VS Code themes and is not packaged with Nulltone.
