# Vectrune TextMate Grammar

TextMate grammar for [Vectrune](https://github.com/davethomas11/vectrune) (`.rune`) files.

Provides syntax highlighting for `.rune` files in editors and platforms that support TextMate grammars, including VS Code, GitHub, GitLab, and others.

## Scope

`source.rune`

## Highlighted

- `@Section` headers (`@App`, `@Route`, `@Page`, `@Logic`, `@Style`, etc.)
- Keywords (`if`, `then`, `else`, `for`, `in`, `return`, `stop`, `action`, `func`, `derive`, etc.)
- Strings, numbers, booleans, and null literals
- `#` line comments
- Template interpolation (`{variable}`, `{obj.prop}`, `{array.[index]}`)
- Operators

## Usage

### VS Code

This grammar is bundled with the [Vectrune VS Code extension](https://github.com/davethomas11/vectrune/tree/main/rune-vscode).

### Linguist / GitHub

This repo is registered as a submodule in [github-linguist/linguist](https://github.com/github-linguist/linguist) to enable `.rune` syntax highlighting on GitHub.

## License

MIT

