# Vectrune TextMate Grammar

TextMate grammar for [Vectrune](https://github.com/davethomas11/vectrune) (`.rune`) files.

Provides syntax highlighting for `.rune` files in editors and platforms that support TextMate grammars, including VS Code, GitHub, GitLab, and others.

## Scope

`source.rune`

## Features

Syntax highlighting for:

### Sections
- `@Section` headers with optional identifiers and qualifiers
  - Basic: `@App`, `@Frontend`, `@Backend`
  - With ID: `@Page/home`, `@Logic/game`, `@Style/board`
  - With HTTP verbs and paths: `@Route/GET /users/{id}`, `@Schema/User`

### Keywords
- Control flow: `if`, `then`, `else`, `for`, `in`, `return`, `stop`, `when`
- Logic: `and`, `or`, `not`
- Special: `from`, `use`, `swap`, `full`

### Definitions
- Actions: `action play(index):`
- Functions: `func win(board, player):`
- Block keywords: `run:`, `state:`, `view:`, `derive:`, `tokens:`, `presets:`, `rules:`

### Built-in Functions
- `respond`, `log`, `validate`
- `parse-json`
- CSV operations: `csv.read`, `csv.write`, `csv.append`

### Literals & Values
- Strings: `"double-quoted"` with escape sequences
- Numbers: `0`, `42`, `3.14`, `-1`
- Booleans and special values: `true`, `false`, `null`, `draw`

### Advanced Syntax
- Template interpolation: `{variable}`, `{obj.prop}`, `{array.[index]}`
- Record assignments: `name = value`, `board.[index] = turn`
- Record markers: `+ entry`
- CSS-style selectors in `@Style` blocks: `.class:`, `element:`
- Operators: `==`, `!=`, `<=`, `>=`, `->`, `=>`, `++`, `--`, `+`, `-`, `*`, `/`, `&`, `|`
- Path placeholders: `%ROOT%`, `%PLACEHOLDER%`
- Shebang: `#!RUNE` (not treated as regular comments)
- `#` line comments

## Usage

### VS Code

This grammar is bundled with the [Vectrune VS Code extension](https://github.com/davethomas11/vectrune/tree/main/rune-vscode).

### Linguist / GitHub

This repo is registered as a submodule in [github-linguist/linguist](https://github.com/github-linguist/linguist) to enable `.rune` syntax highlighting on GitHub.

## License

MIT

