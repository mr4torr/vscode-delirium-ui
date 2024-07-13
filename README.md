# VSCode Delirium UI - Color Themes

[![codecov](https://codecov.io/gh/mr4torr/vscode-delirium-ui/branch/master/graph/badge.svg)](https://codecov.io/gh/mr4torr/vscode-delirium-ui) [![Build Status](https://travis-ci.org/mr4torr/vscode-delirium-ui.svg?branch=master)](https://travis-ci.org/mr4torr/vscode-delirium-ui)

--------------------------------------

<p align="center">
	<a href="https://themes.vscode.one/theme/mr4torr/3ZjBASTu">
		<img src="https://raw.githubusercontent.com/mr4torr/vscode-delirium-ui/main/icon.png" />
	</a>
</p>
<p align="center">
	<a href="https://themes.vscode.one/theme/mr4torr/3ZjBASTu">
		<img src="https://raw.githubusercontent.com/mr4torr/vscode-delirium-ui/main/default.jpeg" />
	</a>
</p>

<b>Everforest Dark</b>
<p align="center">
	<a href="https://themes.vscode.one/theme/mr4torr/3ZjBASTu">
		<img src="https://raw.githubusercontent.com/mr4torr/vscode-delirium-ui/main/everforest.png" />
	</a>
</p>

## Installation

You can install manually from `git` or use the [vscode extensions marketplace](https://marketplace.visualstudio.com/items?itemName=mr4torr.delirium-ui).

### Marketplace Installation

From command palette, run

```
ext install mr4torr.delirium-ui
```

Or search for `Delirium UI` in the marketplace and install from there.

### Git Installation

* Go to `~/.vscode/extensions/`
* Clone the repository.
```bash
git clone git@github.com:mr4torr/vscode-delirium-ui.git
```

### Activation

After installation, open/restart vscode and from command palette search for
`Delirium`. You can choose and apply the color theme of your choice.

## Customization

Workspace colors can be customized by editing `workbench.colorCustomizations`
user settings. More information can be found [here](https://code.visualstudio.com/docs/getstarted/theme-color-reference).

## Recommended Settings

Following extensions/tools are recommended for the color schemes.

* [vscode-icons](https://marketplace.visualstudio.com/items?itemName=robertohuertasm.vscode-icons) - For file icons.
* [WhiteViz](https://marketplace.visualstudio.com/items?itemName=spywhere.whiteviz) - Sublime like whitespace highlight.
* [FiraCoda](https://github.com/tonsky/FiraCode) - For an awesome font with ligatures.
* [Operator Mono Lig](https://github.com/kiliman/operator-mono-lig) - For creating ligatures for operator mono.

Also note the recommended user settings.

```json
{
	"workbench.iconTheme": "vscode-icons",
	"editor.fontFamily": "Operator Mono SSM Lig",
	"editor.lineHeight": 25,
	"editor.fontLigatures": true,
	"explorer.decorations.badges": false,
	"editor.fontSize": 14,
	"editor.letterSpacing": 0.5,
	"editor.fontWeight": "400",
	"editor.renderWhitespace": "none",
	"workbench.statusBar.feedback.visible": false,
	"editor.rulers": [
		80,
		100,
		120
	],
	"whiteviz.maximumLimit": 500,
	"whiteviz.expandedTabIndicator": false,
	"editor.occurrencesHighlight": true,
	"workbench.tree.horizontalScrolling": true,
	"editor.cursorStyle": "line-thin",
	"editor.showFoldingControls": "always",
	"editor.matchBrackets": true
}
```


## Development

> Help porting popular tmThemes to vscode.

The development is made easy with some custom scripts. First fork and clone the
repo and run

```bash
yarn install
```

This will install all dependencies. Then run

```bash
yarn start
```

To build the themes and watch for file changes. You can press <kbd>F5</kbd> to
launch VSCode development window where you can preview the themes.

Once satisfied run

```bash
yarn build
```

to finalize the themes and make changes to `package.json` manually.

Then submit a PR.

### Adding a new theme

* Copy `./src/schemes/Template.noop.js` to `./src/schemes/MyTheme.js`.
* Mark the theme `dark` or `light` and make changes accordingly.
* Add colors to the config.
* Import and add the theme in `src/colors.js`.
* Build and test.

<h1 align="center">
👨‍🎨
</h1>
