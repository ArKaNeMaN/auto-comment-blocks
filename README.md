# Auto Comment Blocks

A simple VS Code extension for C, C++, C#, and Java that ports VS Code's JavaScript block comment completion functionality.

## Usage
![Demo](https://raw.githubusercontent.com/kevinkyang/auto-comment-blocks/master/img/demo.gif)

### Javadoc-style comment blocks
Type `/**` to start a block comment, then hit the Enter key, and the extension will close the block. While inside the comment block, the extension will insert an asterisk at the start of every new line, and align the comment, respecting indentation.

### QDoc-style (Qt) comment blocks
**New feature:** use `/*!` in C/C++ files to start a QDoc comment block.

## Feature requests
Currently, this extension supports C, C++, C#, and Java. If you want to suggest a feature or request support for a specific language, please create an issue in the [repository](https://github.com/kevinkyang/auto-comment-blocks/issues). In the interest of keeping this extension simple and lightweight, some features may not be possible right now.

## Extension Settings

There is one setting for this extension:

* `auto-comment-blocks.languages`: Comment completion will be enabled for the languages in this list. 

## Issues

* Currently, VS Code only allows extensions to overwrite, instead of modify, existing language configurations. This means that this extension may clash with another extension that overwrites the same language configurations, causing one or both not to work. In that case, uninstalling this extension is the only option for now.

Please create an issue in the Github repository if you find any bugs or have questions/requests.

## Release Notes

### 0.0.1
- Initial Release.

### 0.0.4
- Fixed an issue that caused asterisk insertion and indentation bugs when indenting using an odd number of spaces.

### 0.0.5
- Fix major typo that caused an asterisk to be inserted following any indented line.

### 0.1.0
- Add QDoc (Qt-style) comment block completion for C and C++.