<!-- markdownlint-disable MD007 MD025 -->

# Welcome

Dev tips, resources and tools that I came across one day and wanted to share. Updated multiple times a week.
Feel free to make some suggestions !

As this page grows, I will probably change the sections or create separate, dedicated pages by themes.

See also the separate pages like [Mac](/Mac.md) or [VSCode](/VSCode.md).

## Table of Contents

<!-- TOC -->

- [Welcome](#welcome)
    - [Table of Contents](#table-of-contents)
- [Resources/Assets (OpenData, Pictures, Audio, 3D Models...)](#resourcesassets-opendata-pictures-audio-3d-models)
    - [OpenData](#opendata)
    - [3D Models](#3d-models)
    - [Audio](#audio)
    - [Textures](#textures)
- [Languages, Frameworks, Tools](#languages-frameworks-tools)
    - [.NET](#net)
    - [Android](#android)
        - [Getting started](#getting-started)
        - [Useful apps](#useful-apps)
    - [CSS](#css)
    - [Docker](#docker)
        - [Remove all containers, images, volumes](#remove-all-containers-images-volumes)
    - [Java](#java)
        - [Properties file](#properties-file)
    - [Javascript](#javascript)
        - [Best practices](#best-practices)
        - [Interesting readings](#interesting-readings)
        - [Misc](#misc)
            - [Javascript Bind](#javascript-bind)
    - [LaTeX](#latex)
    - [Markdown](#markdown)
        - [Inserting multiple empty lines](#inserting-multiple-empty-lines)
    - [Node.js](#nodejs)
    - [PowerShell](#powershell)
    - [Python](#python)
    - [Regex](#regex)
    - [Scala](#scala)
        - [Learning and Training](#learning-and-training)
        - [Various Q&A](#various-qa)
- [IDEs, text editors](#ides-text-editors)
    - [IntelliJ](#intellij)
        - [Plugins](#plugins)
    - [Unity3D (Game Engine)](#unity3d-game-engine)
    - [VIM](#vim)
    - [Visual Studio Code](#visual-studio-code)
- [Prototyping/Designing tools](#prototypingdesigning-tools)
- [Other](#other)
    - [Git](#git)
        - [Aliases](#aliases)
        - [.gitignore templates](#gitignore-templates)
        - [Configure pull to use rebase](#configure-pull-to-use-rebase)
        - [Reduce the size of .git folder](#reduce-the-size-of-git-folder)
        - [Clone only one branch](#clone-only-one-branch)
        - [Filenames capitalization](#filenames-capitalization)
    - [GitHub](#github)
        - [GitHub Pages](#github-pages)
    - [Licenses](#licenses)
    - [Miscellaneous](#miscellaneous)
        - [How to know if a string is a MD5 or a SHA1 checksum](#how-to-know-if-a-string-is-a-md5-or-a-sha1-checksum)
    - [Interesting Open Source Repos](#interesting-open-source-repos)
    - [Slack](#slack)
        - [Nice tools](#nice-tools)
- [Better quality code tools](#better-quality-code-tools)
    - [Windows Troubleshooting](#windows-troubleshooting)

<!-- /TOC -->

&nbsp;

# Resources/Assets (OpenData, Pictures, Audio, 3D Models...)

Unless specified, these are free resources.

## OpenData

[OpenData.swiss](https://opendata.swiss/fr/)\
[CERN Open Data Portal](http://opendata.cern.ch/)

## 3D Models

[Free3D](https://free3d.com/) : free models
[Archive3D](https://archive3d.net/) : free models
[Turbosquid](https://www.turbosquid.com/) : paid and free models

## Audio

[Freesound.org](https://www.freesound.org/)\
[OpenMusicArchive.org](http://openmusicarchive.org/)

## Textures

[Textures.com](https://www.textures.com/)
[My-textures.com](http://my-textures.com) : Free textures for personal and commercial use
[Myfreetextures.com](http://www.myfreetextures.com)
[Texturegen.com](http://www.texturegen.com)
[Texturelib.com](http://texturelib.com)
[Plaintextures.com](http://www.plaintextures.com)

&nbsp;

# Languages, Frameworks, Tools

## .NET

[Naming Guidelines](https://msdn.microsoft.com/en-us/library/ms229002(v=vs.110).aspx)\
Naming conventions of the .NET framework : Capitalization conventions, general naming conventions, names of classes, interfaces, type members etc.

## Android

### Getting started

[Android Jetpack](https://developer.android.com/jetpack/):  A set of libraries, tools and architectural guidance to help make it quick and easy to build Android apps.

### Useful apps

[AZ Screen Recorder](https://play.google.com/store/apps/details?id=com.hecorat.screenrecorder.free)\
Records the screen and the audio played on device.

## CSS

[CSS Diner](https://flukeout.github.io/) : interactive learning of CSS selectors (how to select elements by their class, id, last element...).
[Flexible Box (Flexbox) MDN documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout)

## Docker

[Dockerfile best practices](https://docs.docker.com/engine/userguide/eng-image/dockerfile_best-practices/)

[Docker cheat sheet](https://github.com/wsargent/docker-cheat-sheet)

[Understand the concept of Image and Layer](https://stackoverflow.com/a/45611871/1975002) | [About images, containers, and storage drivers](https://docs.docker.com/engine/userguide/storagedriver/imagesandcontainers/#container-size-on-disk)

### Remove all containers, images, volumes

Stop all running containers : `docker stop $(docker ps -a -q)`\
`docker system prune -a --volumes` [(documentation)](https://docs.docker.com/engine/reference/commandline/system_prune/#examples)

## Java

### Properties file

[Simple tutorial to write and read properties file](https://www.mkyong.com/java/java-properties-file-examples/)

## Javascript

### Best practices

[JavaScript - The Right Way](http://jstherightway.org/) : Best practices for JS. Coding style, tools, frameworks...\
[Idiomatic.js](https://github.com/rwaldron/idiomatic.js) : A guide to write consistent, idiomatic JavaScript.

### Interesting readings

[JavaScript: The Good Parts [Douglas Crockford]](http://shop.oreilly.com/product/9780596517748.do)

### Misc

#### Javascript Bind

[Really nice explanation about 'Bind' on SO](https://stackoverflow.com/a/10115970/1975002)\
[bind() function documentation on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/bind)

## LaTeX

[todonotes](https://ctan.org/pkg/todonotes) : a simple way to add todo notes to a document. They appear on the right margin by default.

## Markdown

[CommonMark](http://commonmark.org)\
*A strongly defined, highly compatible specification of Markdown*. Now also [used by GitHub in place of GFM](https://githubengineering.com/a-formal-spec-for-github-markdown).
[Markdowntutorial.com](https://www.markdowntutorial.com/): interactive tutorial for learning Markdown.

### Inserting multiple empty lines

This can be done by using the non-breaking space character : `&nbsp;`\
(Alternatively, you can use `<br>`)

## Node.js

List all packages that are installed as well as thier dependencies : `npm list [-g] [--depth=0]`
See outdated packages : `npm [-g] outdate`

## PowerShell

[posh-git](https://github.com/dahlbyk/posh-git): a PowerShell module that integrates Git and PowerShell by providing Git status summary information that can be displayed in the PowerShell prompt.\
posh-git also provides tab completion support for common git commands, branch names, paths and more.

## Python

[Enforce arguments to a specific list of values](https://stackoverflow.com/questions/25854380/enforce-arguments-to-a-specific-list-of-values)\
[Generating list of lists](https://stackoverflow.com/questions/240178/list-of-lists-changes-reflected-across-sublists-unexpectedly)

## Regex

[Regex Crossword](https://regexcrossword.com/) : puzzle challenges from beginner to expert to learn and train Regex.

[Regex101](https://regex101.com/) : online regex editor and debugger. Allows to create, debug, test and have expressions explained for PHP, PCRE, Python, Golang and JavaScript.\
[RegExr](https://regexr.com/) : Learn, build & test Regular Expressions.

## Scala

[Naming conventions](https://docs.scala-lang.org/style/naming-conventions.html)

### Learning and Training

[Scala Exercices](https://www.scala-exercises.org)\
[Alvin Alexander's Scala tutorials](http://alvinalexander.com/scala/)\
[Twitter's Scala School](https://twitter.github.io/scala_school/)\
[S-99 : Ninety-nine Scala Problems](http://aperiodic.net/phil/scala/s-99/)

### Various Q&A

Q: What is the difference between == and .equals in Scala ?\
A: You normally use ==, it routes to equals, except that it treats nulls properly. Reference equality (rarely used) is eq. [(source, other answers are also interesting)](https://stackoverflow.com/a/7681243/1975002)

Q: List concatenation, ::: vs ++ ?\
A: [Answer (three first answers)](https://stackoverflow.com/q/6559996/1975002)

&nbsp;

# IDEs, text editors

## IntelliJ

### Plugins

[.ignore](https://plugins.jetbrains.com/plugin/7495--ignore)\
Plugin for .\*ignore files (e.g.: &nbsp;*.gitignore*). Files syntax highlight, coloring ignored files in the Project View, suggestion of default *.gitignore* file for new project, and other useful functionalities.

## Unity3D (Game Engine)

[Unity3d Best practices](https://unity3d.com/fr/learn/tutorials/s/best-practices)

[Unity3D on Linux](https://forum.unity.com/threads/unity-on-linux-release-notes-and-known-issues.350256/) : Where to get the latest builds, release notes and known issues.

[Special folder names in Assets folder](http://wiki.unity3d.com/index.php/Special_Folder_Names_in_your_Assets_Folder)\
Explain for example the special "Resources" folder.\
[StreamingAssets folder](https://docs.unity3d.com/Manual/StreamingAssets.html) : Any files placed in a folder called StreamingAssets (case-sensitive) in a Unity project will be copied verbatim to a particular folder on the target machine.[...]

## VIM

[VIM Adventures](https://vim-adventures.com/): a game to learn VIM

## Visual Studio Code

=> See the dedicated [VS Code section](/VSCode.md).

&nbsp;

# Prototyping/Designing tools

[Balsamiq](https://balsamiq.com/) wireframing\
[Ziteboard](https://ziteboard.com/) online collaborative whiteboard

# Other

Stuffs that needs to be ordered one time...

[Pandoc.org](http://pandoc.org/) : a universal document converter. Converts files from various markup format into another.

## Git

[How to write a git commit message](https://chris.beams.io/posts/git-commit/): A must-read article on good practices about writing useful, nice git commit messages. (Thanks [@jcavat](https://github.com/jcavat) for sharing !)

### Aliases

[Must have Git Aliases](http://durdn.com/blog/2012/11/22/must-have-git-aliases-advanced-examples/) : nice samples of git aliases. Basic shortcuts are also listed at the end.

### .gitignore templates

[GitHub's templates collection](https://github.com/github/gitignore)\
The .gitignore templates as offered in the GitHub.com interface when creating new repositories and files.

[gitignore.io](https://www.gitignore.io/)\
Just type the name of the IDE or programming language and get the corresponding *.gitignore* file.

### Configure pull to use rebase

```bash
git config pull.rebase true # for current repository, add `--global` for all
```

### Reduce the size of .git folder

```bash
git gc
```

This command remove unnecessary files and optimize the local repository. See [git-gc manual page](https://www.kernel.org/pub/software/scm/git/docs/git-gc.html)

### Clone only one branch

```bash
git clone -b branch_name --single-branch https://domain.com/repo.git
```

### Filenames capitalization

[Changing capitalization of filenames in Git](https://stackoverflow.com/questions/10523849/changing-capitalization-of-filenames-in-git/24979063#24979063)

## GitHub

[DownGit](https://minhaskamal.github.io/DownGit/#/home): tired of cloning a whole repository when you just need some specific files/folders ? Just past the link to the resource you need and DownGit will make a .zip file of it, ready to download.\

[Removing sensitive data from a repository](https://help.github.com/articles/removing-sensitive-data-from-a-repository/)

### GitHub Pages

[GitHub Pages examples](https://github.com/collections/github-pages-examples)
[Dr. Jekyll's Themes](https://drjekyllthemes.github.io/): jekyll themes directory

## Licenses

[Choose a license](https://choosealicense.com/) : simple explanations to help choosing the appropriate license for a project.

## Miscellaneous

[Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet/)

[Semantic Versioning](http://semver.org/)

[Microsoft REST API Guidelines](https://github.com/Microsoft/api-guidelines/blob/vNext/Guidelines.md#72-url-length)

### How to know if a string is a MD5 or a SHA1 checksum

It depends of the length : 128-bit sequence (32 hexadecimal digits) => possible MD5 hash, 160-bit (40 hex digits) sequence => possible SHA1 hash.

## Interesting Open Source Repos

[Microsoft Open Source](https://opensource.microsoft.com/) : all the open-source repos from Microsoft. Personal selection :

- [TypeScript-React-Start](https://github.com/Microsoft/TypeScript-React-Starter)

## Slack

### Nice tools

[Simple Poll](https://simplepoll.rocks/)

# Better quality code tools

Code coverage, CI...

[Coveralls](https://coveralls.io/): Shows which part of code aren't covered by the test suite. Free for open source repos.

## Windows Troubleshooting

[SysInternals Live](https://live.sysinternals.com/)
