# GitHub Soft Theme

A modern light theme for [Visual Studio Code](http://code.visualstudio.com/) with lower saturation colors. Designed to be easy on the eyes. Based on [GitHub Theme](https://marketplace.visualstudio.com/items?itemName=GitHub.github-vscode-theme). Other sources of inspiration are [Nord](https://marketplace.visualstudio.com/items?itemName=arcticicestudio.nord-visual-studio-code), [Nord Light](https://marketplace.visualstudio.com/items?itemName=huytd.nord-light), [Night Owl](https://marketplace.visualstudio.com/items?itemName=sdras.night-owl) and [Vitesse Theme](https://marketplace.visualstudio.com/items?itemName=antfu.theme-vitesse).

The theme also offers a flatter UI with a uniform white background color for editor, panel and sidebar.

## Installation

Using CLI:

```sh
code --install-extension IgorKrupenja.vscode-github-soft-theme
```

Or from the VSCode Marketplace:

1. Open the [theme page on VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=IgorKrupenja.vscode-github-soft-theme).
2. Click on the "Install" button and wait for the installation to complete.
3. Choose "GitHub Soft" from the list that appears.

## Screenshots

### TypeScript

![GitHub Soft Theme with TypeScript](images/screenshot-ts.png)

### React TSX

![GitHub Soft Theme with React TSX](images/screenshot-tsx.png)

### SCSS, panel and sidebar

![GitHub Soft Theme with SCSS](images/screenshot-scss.png)

## Recommended settings for other extensions

### [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)

```json
"material-icon-theme.saturation": 0.6,
```

### [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)

```json
"todohighlight.defaultStyle": {
  "color": "#A74047",
  "backgroundColor": "#A7404730",
  "overviewRulerColor": "#A74047",
  "borderRadius": "2px"
},
```

### [Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)

```json
"importCost.largePackageLightColor": "#A74047AA",
"importCost.mediumPackageLightColor": "#DBAB09AA",
"importCost.smallPackageLightColor": "#22863AAA",
```

### [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)

```json
"git-graph.graph.colours": [
  "#D73A4A",
  "#28A745",
  "#DCAB07",
  "#0366D6",
  "#5B32A3",
  "#1C7C82"
],
```

### [Quokka](https://marketplace.visualstudio.com/items?itemName=WallabyJs.quokka-vscode)

```json
"quokka.colors": {
  "covered": "#22863A",
  "notCovered": "#959DA5",
  "partiallyCovered": "#DBAB09",
  "errorSource": "#D73A49",
  "errorPath": "#F97583"
},
"quokka.lightTheme.log.decorationAttachmentRenderOptions": {
  "color": "#005CC5"
},
"quokka.lightTheme.system.decorationAttachmentRenderOptions": {
  "color": "#6A737D"
},
"quokka.lightTheme.error.decorationAttachmentRenderOptions": {
  "color": "#D73A49"
},
```

### [Jumpy2](https://marketplace.visualstudio.com/items?itemName=DavidLGoldberg.jumpy2)

Note that these have to be set through `workbench.colorCustomizations` and can be set per-theme, e.g.:

```json
"workbench.colorCustomizations": {
  "[GitHub Soft]": {
    "jumpy2.labelFontColor": "#FFFFFF",
    "jumpy2.labelBackgroundColor": "#5a32a3",
    "jumpy2.labelBorderColor": "#5a32a3",
    "jumpy2.checkered_labelFontColor": "#FFFFFF",
    "jumpy2.checkered_labelBackgroundColor": "#5a32a3",
    "jumpy2.checkered_labelBorderColor": "#5a32a3"
  }
},
```

## Customization

To customize this theme, refer to the [color theme documentation](https://code.visualstudio.com/api/extension-guides/color-theme). For a detailed list of available color customizations, see [theme color reference](https://code.visualstudio.com/api/references/theme-color). This allows you to conveniently make minor adjustments to the theme without the need to create and manage your own theme repository.

### Editor syntax highlighting

You can also [customise editor syntax highlighting](https://code.visualstudio.com/docs/getstarted/themes#_editor-syntax-highlighting). An example:

```json
"editor.tokenColorCustomizations": {
  "[GitHub Soft]": {
    "textMateRules": [
      {
        "scope": ["variable.object.property.tsx"],
        "settings": { "foreground": "#ff0000" }
      }
    ]
  }
}
```

### Semantic highlighting

[Semantic highlighting](https://code.visualstudio.com/api/language-extensions/semantic-highlight-guide) is **disabled** for this theme by default. I found the feature too flashy and distracting. If you want to enable it, add the following to your settings:

```json
"editor.semanticHighlighting.enabled": true,
```

It can also be enabled per-language if needed, for example:

```json
"[typescript]": {
  "editor.semanticHighlighting.enabled": true
},
```

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for details.

### 1.2.7

- Fix version info in Readme and changelog.

### 1.2.6

- Reduce packaged extension size 50x by removing unnecessary files.

### 1.2.5

- Fix typo in Readme.

### 1.2.3

- Fix version info in Readme and changelog.

### 1.2.1

- Fixed a broken link and other minor issues in Readme.
- Added recommended colors for [Jumpy2 extension](https://marketplace.visualstudio.com/items?itemName=DavidLGoldberg.jumpy2).

### 1.2.0

- Made git conflicted resource color less saturated.

### 1.1.0

- Made editor ruler color match other theme colors.
- Made editor range highlight color (`editor.rangeHighlightBackground`) less saturated.
- Made GraphQL syntax highlighting colors less saturated.
- Changed type color to brown(ish) to make it more distinct and have brightness better matching other colors. Previously it was too similar to the color of unused variables.
- Made TS/TSX primitive type color match other types.
- Made [testing colors](https://code.visualstudio.com/api/references/theme-color#testing-colors) match other theme colors.

## Feedback

If you like the theme, please add a review here or star on [GitHub](https://github.com/IgorKrupenja/vscode-github-soft-theme).

If you have suggestions, please open an [issue](https://github.com/IgorKrupenja/vscode-github-soft-theme/issues/new) or, even better, a [pull request](https://github.com/IgorKrupenja/vscode-github-soft-theme/pulls).

You can also create issues or Readme PRs for other extensions that you think should be included in the recommended settings.
