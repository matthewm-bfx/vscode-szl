# Sizzle for VS Code

Syntax highlighting for SynthEyes Sizzle (`.szl`) scripts.

Features:

- Keywords, operators, numbers, strings with escape sequences and printf format
  specifiers, comments, `INCLUDE(...)` directives, and function definitions.
- Builtin functions, object lists (`Scene`, `Trk`, `Obj`, ...) and constants.
- Embedded boilerplate text: text between `]@` and `@[` is highlighted as
  literal output. Exporters (`//SIZZLEX` header) start in boilerplate mode, as
  they do in SynthEyes.
- Line comment toggling, bracket matching, auto-indent and folding of
  `function`/`if`/`for`/`while` ... `end` blocks.

## Installation

Package and install with [vsce](https://github.com/microsoft/vscode-vsce):

    npx @vscode/vsce package
    code --install-extension sizzle-0.1.0.vsix

Or, for development, link this directory into your extensions folder
(`~/.vscode/extensions/`, or `%USERPROFILE%\.vscode\extensions` on Windows) and
restart VS Code.
