# VS Code Universal Templates Syntax

> This extension is meant for internal template development and not intended for public usage.

## Features

Working with novel systems can sometimes be hard on developer productivity and efficiency. This project aims to boost DX with internal templates for BS-Production. Starting with this extension developers can benefit from VS Code's syntax highlighting and extension ecosystem to develop custom templates. With proper syntax highlighting and IntelliSense developers produce better quality code, create fewer buggy implementations and can iterate at _super_ speeds.

Currently, syntax highlighting is supported for the following languages:

- Scripts
  - Javascript (Supported by default)
  - Typescript
  - Coffee script
- Styles
  - CSS (Supported by default)
  - Less
  - Sass
  - Scss
  - Stylus
  - PostCSS

> Intellisense for scripts and styles are coming soon

## Showcase

### Syntax Highlighting

#### HTML, Typescript, Scss

![HTML, Typescript, Scss](/assets/showcase/html-ts-scss.png)

#### HTML, Coffee Script, Sass

![HTML, Coffee, Sass](/assets/showcase/html-coffee-sass.png)

## Roadmap

- [ ] Add support for intellisense, hovers and validators (https://code.visualstudio.com/docs) (Consider using Request forwarding)
- [ ] More language syntax support (current selection seems for a good start)
- [ ] Consider supporting parent file extensions (.html vs .ut)

## Folders Explained & Files

- This folder contains all of the files necessary for your extension.
- `package.json` - this is the manifest file in which you declare your language support and define the location of the grammar file that has been copied into your extension.
- `syntaxes/.tmLanguage.json` - this is the Text mate grammar file that is used for tokenization.
- `language-configuration.json` - this is the language configuration, defining the tokens that are used for comments and brackets. (Not needed so far)

## Local development of this extension

- Open the folder containing this extension in VS Code
- Press `F5` to open a new window with your extension loaded.
- Create a new file with a file name suffix matching your language.
- Verify that syntax highlighting works.

### Making changes

- You can relaunch the extension from the debug toolbar after making changes to the files listed above.
- You can also reload (`Ctrl+R` or `Cmd+R` on Mac) the VS Code window with your extension to load your changes.

## Install this extension

- To start using this extension with VS Code copy it into the `<user home>/.vscode/extensions` folder and restart VS Code.

## Release Notes

> Currently still in the testing phase

### 0.0.1

Initial proof of concept. This release focuses heavily on only adding syntax highlighting for supported languages of the UT-bundler. languages added:

- Scripts
  - Javascript (Supported by default)
  - Typescript
  - Coffee script
- Styles
  - CSS (Supported by default)
  - Less
  - Sass
  - Scss
  - Stylus
  - PostCSS
