# Introduction

I'm in love with [VS Code](https://code.visualstudio.com/) ! I think it's an awesome code editor, highly extensible and customizable.\
VS Code is [open source](https://github.com/Microsoft/vscode), runs on Linux, Mac and Windows, and has a wide community. The dev team is really reactive and communicates well about the new features and improvements made month after month.

I'm sharing there my favorites extensions, some tips and stuffs I've found while using this great tool.

## Extensions

Homepage : [VS Code Marketplace](https://marketplace.visualstudio.com/VSCode)

### Syncing VSCode settings and extensions

[Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync) : uses your GitHub account and Gist to sync your preferences and installed extensions.\
`Shift + Alt + U` to upload your settings.\
`Shift + Alt + D` to download your settings.

### LaTeX

[LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)

### Markdown

[markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) : Markdown linting and style checking for Visual Studio Code

To disable one or more rules in a file, add this line : `<!-- markdownlint-disable MD001 MD002 -->`\
(MDxxx are the rules identifiers)

[Markdown TOC](https://marketplace.visualstudio.com/items?itemName=AlanWalk.markdown-toc): Generate TOC (table of contents) of headlines from parsed markdown file.

## Themes

[VS Code documentation - Themes](https://code.visualstudio.com/docs/getstarted/themes)\
[Darcula Theme](https://marketplace.visualstudio.com/items?itemName=rokoroku.vscode-theme-darcula) => `ext install vscode-theme-darcula`
[Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme): provides lots of nice Material Design icons.

## Working with Markdown files in VS Code

[Markdown and VS Code](https://code.visualstudio.com/docs/languages/markdown)

View the preview : `Ctrl+Shift+V`\
View the preview side-by-side : `Ctrl+K  V`

## Some useful settings

Set default end-of-line as LF : `"files.eol": "\n"` (`"\r\n"` for CRLF)