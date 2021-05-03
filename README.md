# Asteria

Introducing BiancoNero, a minimal, black and white theme for day and night.

> Note: This is a work in progress.

[![Version](https://vsmarketplacebadge.apphb.com/version/spaceinvadev.bianconero.svg)](https://marketplace.visualstudio.com/items?itemName=spaceinvadev.bianconero)

![Logo of the Bianconero theme](/images/bianconero-logo.png)

<br>

## Installation

1. Open the **Extensions** sidebar panel in VS Code. `View → Extensions`

2. Search for `BiancoNero`

3. Click `Install`

4. When prompted, select `BiancoNero` as the color theme

> In case of not being prompted to select a Color Theme upon installing, go to the menu bar and select: `Code (File, on Windows) > Preferences > Color Theme > BiancoNero`. Alternatively, you can use the shortcut `⌘/Ctrl + K > ⌘/Ctrl + T` and select `BiancoNero`.

<br>

### Recommended settings for a better experience

The typeface I used (as shown on the sample images) is **MD IO** — my new preferred typeface for coding. You can get it from [Future Fonts](https://www.futurefonts.xyz/mass-driver/io). I use some custom, personal typography-related settings, which you can achieve by adding the following to your `settings.json` file.

```json
// Controls the font family
"editor.fontFamily": "'MD IO 0.2', monospace",

// Controls the font size in pixels
"editor.fontSize": 16,

// Controls letter spacing in pixels
"editor.letterSpacing": -0.8,

// Controls the font weight
"editor.fontWeight": 400,

// Controls the line height. Use 0 to compute the line height from the font size
"editor.lineHeight": 32,

// Enables/Disables font ligatures
"editor.fontLigatures": true
```

<br>

### Customize/Override theme colors

You can customize/override the BiancoNero theme colors by adding the following theme-specific configuration to your settings file. For more advanced customization, refer to the corresponding [VS Code Docs](https://code.visualstudio.com/docs/getstarted/themes#_customizing-a-color-theme).

<br>

#### Example of basic customization

```json
"editor.tokenColorCustomizations": {
  "[BiancoNero]": {
      "comments": "#229977"
  }
},
```

<br>

#### Example of advanced customization

```json
"editor.tokenColorCustomizations": {
  "[Your_Custom_BiancoNero]": {
    "textMateRules": [
      {
        "scope": [
          "punctuation.definition.comment",
          "comment.block",
          "comment.line",
          "comment.block.documentation"
        ],
        "settings": {
          "foreground": "#ffff00"
        }
      }
    ]
  },
},

"workbench.colorCustomizations": {
  "[Your_Custom_BiancoNero]": {
    "sideBar.background": "#ffff00",
  }
},
```

<br>

## Contributions, Issues & Suggestions

Any feedback, issue reporting or suggestion is welcome. Feel free to submit your concern via the [Repo's GitHub Issues](https://github.com/spaceinvadev/bianconero/issues) page, provide feedback or request a feature by submitting a PR.

<br>

## Changelog

All notable changes to this project are documented in the [changelog](CHANGELOG.md). Consider checking the changelog prior to filing any issues as they may have already been addressed.
