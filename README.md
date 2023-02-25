# Clang-Format Indent 4 for VS Code

[![License: MIT](https://img.shields.io/badge/license-MIT-orange.svg)](https://github.com/xaverh/vscode-clang-format/blob/master/LICENSE) [![Marketplace](https://img.shields.io/badge/marketplace-vscode-blue)](https://marketplace.visualstudio.com/items?itemName=demiaochen.clang-format-indent-4)

## Code Formatter

Use clang-format to format your C/C++/Java/JavaScript/Objective-C/Objective-C++/Protobuf with indentations of 4 spaces like the following:

```cpp
if (int i = 0; i < n; ++i) {
    while (true) {
        foo();
    }
} else {
    baz();
}
```

## Acknowledgement

The extension is forked from <https://github.com/xaverh/vscode-clang-format-provider> and modified to use clang-format with indent 4. More usage details can be found in the original repo.

## Usage

Install clang-format:

``` bash
npm install -g clang-format
```

Get absolute path to clang-format:

```bash
which clang-format
```

Add the following to your vscode `settings.json` file (open with `Ctrl/CMD+Shift+P` and select `Preferences: Open Settings (JSON)`):

```json
{
  "clang-format.executable": "/absolute/path/to/clang-format",
}
`````

To automatically format a file on save, add the following to your vscode `settings.json` file (example for C++):

```json
{
  "editor.formatOnSave": true,
  "[cpp]": {
    "editor.defaultFormatter": "demiaochen.clang-format-indent-4",
  }
}
```

## Clang-Format

[Clang-Format](http://clang.llvm.org/docs/ClangFormat.html) is a tool to format C/C++/Java/JavaScript/Objective-C/Objective-C++/Protobuf code. It can be configured with a config file named `.clang-format` within the working folder or a parent folder. Configuration see: <http://clang.llvm.org/docs/ClangFormatStyleOptions.html>

## Source code

Available on github: <https://github.com/demiaochen/vscode-clang-format-indent-4>
