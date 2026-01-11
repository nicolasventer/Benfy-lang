# Benfy Lang

A VS Code extension that provides syntax highlighting and language support for Benfy Lang (`.bf` files).

## Features

- **Syntax Highlighting**: Full syntax highlighting for Benfy Lang files
- **Language Support**: Recognizes `.bf` file extensions
- **Grammar Rules**: Supports rule definitions, regex patterns, symbols, and comments
- **Auto-completion**: Basic language configuration with brackets and quotes auto-closing

## Supported Syntax Elements

The extension provides syntax highlighting for:

- **Rule Names**: Identifiers at the start of a line (e.g., `rule_name`, `RuleName`)
- **Rule References**: Function-like references anywhere in the code (e.g., `rule_ref`)
- **Regex Patterns**: Regular expressions enclosed in forward slashes with optional flags (e.g., `/pattern/`, `/pattern/s`, `/pattern/slmi`)
  - Supported flags: `s`, `l`, `m`, `i`
- **Symbols**: Control operators (`:`, `>>`, `?`, `+`, `*`, `!`, `|`)
- **Spacing Policy**: Keywords `"strict"` or `"loose"`
- **Comments**: 
  - Single-line comments starting with `#`
  - Multi-line comments enclosed in `##` ... `##`

## Installation

### From VS Code Marketplace
1. Open VS Code
2. Go to Extensions (Ctrl+Shift+X)
3. Search for "Benfy Lang"
4. Click Install

### From Source
1. Clone this repository
2. Open the project in VS Code
3. Press `F5` to run the extension in a new Extension Development Host window

## Usage

1. Open any `.bf` file in VS Code
2. The extension will automatically activate and provide syntax highlighting
3. Enjoy enhanced code readability with proper syntax coloring

## Language Configuration

The extension includes:
- Auto-closing brackets: `{}`, `[]`, `()`
- Auto-closing quotes: `"`, `'`
- Comment support: `#` for line comments, `##` for block comments

## Example Benfy Lang File

```bf
# This is a single-line comment
## This is a
   multi-line comment ##

rule_name >> /pattern/ | another_rule
RuleName : /pattern_with_flags/slmi
rule_ref ? /regex_pattern/
symbol_test + /test/ * /multiple/ ! /negation/
spacing "strict"
```

## Development

### Prerequisites
- Node.js
- VS Code
- Git

### Building
```bash
npm install
npm run compile
```

### Testing
```bash
npm test
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for a list of changes and version history.

## Issues

If you encounter any issues or have feature requests, please file them on the [GitHub Issues](https://github.com/your-username/benfy-lang/issues) page.

## Support

For support and questions:
- Open an issue on GitHub
- Check the documentation
- Review existing issues and discussions

---

**Benfy Lang** - Making parser development more enjoyable in VS Code! 🚀
