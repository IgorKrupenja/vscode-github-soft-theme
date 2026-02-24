# Changelog

## 1.3.0

- Fixed TypeScript inherited class name color (`implements ClassName`) to match other type names ([#36](https://github.com/IgorKrupenja/vscode-github-soft-theme/issues/36)).
- Fixed YAML `!(...)` expressions (e.g. GitHub Actions `!contains(...)`) no longer rendering as italic red ([#39](https://github.com/IgorKrupenja/vscode-github-soft-theme/issues/39)).
- Fixed SVG path command letters (M, L, C, Z, etc.) no longer rendering in bright pink ([#35](https://github.com/IgorKrupenja/vscode-github-soft-theme/issues/35)).
- Added recommended color settings for [Quokka](https://marketplace.visualstudio.com/items?itemName=WallabyJs.quokka-vscode) extension to Readme ([#41](https://github.com/IgorKrupenja/vscode-github-soft-theme/issues/41)).
- Improved markdown preview inline code colors: added `textPreformat.background` and updated foreground to match GitHub style ([#8](https://github.com/IgorKrupenja/vscode-github-soft-theme/issues/8)).
- Added Peek view screenshot to Readme ([#26](https://github.com/IgorKrupenja/vscode-github-soft-theme/issues/26)).

## 1.2.7

- Fix version info in Readme and changelog.

## 1.2.6

- Reduce packaged extension size 50x by removing unnecessary files.

## 1.2.5

- Fix typo in Readme.

## 1.2.3

- Fix version info in Readme and changelog.

## 1.2.1

- Fixed a broken link and other minor issues in Readme.
- Added recommended colors for [Jumpy2 extension](https://marketplace.visualstudio.com/items?itemName=DavidLGoldberg.jumpy2).

## 1.2.0

- Made git conflicted resource color less saturated.

## 1.1.0

- Made editor ruler color match other theme colors.
- Made editor range highlight color (`editor.rangeHighlightBackground`) less saturated.
- Made GraphQL syntax highlighting colors less saturated.
- Changed type color to brown(ish) to make it more distinct and have brightness better matching other colors. Previously it was too similar to the color of unused variables.
- Made TS/TSX primitive type color match other types.
- Made [testing colors](https://code.visualstudio.com/api/references/theme-color#testing-colors) match other theme colors.

## 1.0.2

- Fixed grammar and formatting in Readme.

## 1.0.1

- Fixed typo in Editor syntax highlighting in Readme.

## 1.0.0

- Fixed capitalisation mistake in theme name, replaced "Github" with "Git**H**ub". Note that this could be a breaking change for some. If you are having issues, please check your settings and update the theme name accordingly. In particular, `workbench.colorTheme` and `workbench.preferredLightColorTheme`. If you had any customizations, also check `editor.tokenColorCustomizations` and `workbench.colorCustomizations`.
- Made breakpoint icon less saturated to match theme colors.
- Modified peek view colors to match theme colors.
- Modified progress bar color to match theme colors.

## 0.2.3

- Fixed typo in Readme.

## 0.2.2

- Made terminal cursor and default text color off-black.
- Made notification background white.
  
## 0.2.1

- Fixed editor colors.
  
## 0.2.0

- Added suggestions for [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph) extension.
- Changed object property color to a less saturated one.

## 0.1.7

- Fixed colors of some active element indicators.
- Fixed title bar border color.

## 0.1.6

- Updated screenshots.

## 0.1.4

- Swapped normal and hover colors for buttons and links.
- Updated theme icon.

## 0.1.3

- Fixed theme path.

## 0.1.2

- Renamed theme.

## 0.1.1

- Fixed Readme and Marketplace banner.

## 0.1.0

- Initial release 🚀
