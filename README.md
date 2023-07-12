# GitHub Soft Theme

A modern light theme for [Visual Studio Code](http://code.visualstudio.com/) with lower saturation colors. Designed to be easy on the eyes. Based on [GitHub Theme](https://marketplace.visualstudio.com/items?itemName=GitHub.github-vscode-theme). Other sources of inspiration are [Nord](https://marketplace.visualstudio.com/items?itemName=arcticicestudio.nord-visual-studio-code), [Nord Light](https://marketplace.visualstudio.com/items?itemName=huytd.nord-light) and [Vitesse Theme](https://marketplace.visualstudio.com/items?itemName=antfu.theme-vitesse).

The theme also offers a flatter UI with a uniform white color for editor, panel and sidebar backgrounds.

## Breaking changes ⚠️

Theme name was slightly changed in version 1.0.0. This might require some settings changes, please have a look below [for details](#100).

## Install

1. Open the theme page on [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=IgorKrupenja.vscode-github-soft-theme).
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

## Customization

To customize this theme, refer to the [color theme documentation](https://code.visualstudio.com/api/extension-guides/color-theme). A detailed list of available color customizations is [here](https://code.visualstudio.com/api/references/theme-color). This allows you to conveniently make minor adjustments to the theme without the need to create and manage your own theme repository.

### Editor syntax highlighting

You can also [customise editor syntax highlighting](https://code.visualstudio.com/docs/getstarted/themes#_editor-syntax-highlighting). An example:

```json
"editor.tokenColorCustomizations": {
  "[GitHub Light Soft]": {
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

[Semantic highlighting](https://code.visualstudio.com/api/language-extensions/semantic-highlight-guide) is **disabled** for this theme by default. I found the feature too colorful and distracting. If you want to enable it, add the following to your settings:

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

## 1.0.0

- Fixed capitalisation mistake in theme name, replaced "Github" with "Git**H**ub". Note that this could be a breaking change for some. If you are having issues, please check your settings and update the theme name accordingly. In particular, `workbench.colorTheme` and `workbench.preferredLightColorTheme`. If you had any customizations, also check `editor.tokenColorCustomizations` and `workbench.colorCustomizations`.
- Made breakpoint icon less saturated to match theme colors.
- Modified peek view colors to match theme colors.
- Modified progress bar color to match theme colors.

### 0.2.3

- Fixed typo in Readme.

### 0.2.2

- Made terminal cursor and default text color off-black.
- Made notification background white.

## To do

- Investigate changing markdown preview code block colors, [#8](https://github.com/IgorKrupenja/vscode-github-soft-theme/issues/8)

## Feedback

If you like the theme, please add a review here or star on [GitHub](https://github.com/IgorKrupenja/vscode-github-soft-theme).

If you have suggestions, please open an [issue](https://github.com/IgorKrupenja/vscode-github-soft-theme/issues/new) or, even better, a [pull request](https://github.com/IgorKrupenja/vscode-github-soft-theme/pulls).

You can also create issues or Readme PRs for other extensions that you think should be included in the recommended settings.
