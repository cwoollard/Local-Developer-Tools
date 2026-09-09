# Local Developer Tools

A single-file, local-first developer toolbox inspired by the classic FreeFormatter.com utilities.

## Why this exists

For a long time, FreeFormatter's simple paste-and-click tools were a useful part of many developers' daily workflows: format JSON, escape a string, encode Base64, convert a timestamp, test a regular expression, and move on.

This project is an independent, from-scratch replacement that keeps that spirit alive. It is **not affiliated with FreeFormatter** and does not copy the original site's branding or implementation.

A small homage is built into the app's **About & homage** panel.

## Privacy

Everything in this version runs in the browser. There is no application server, login, analytics code, API call or upload endpoint.

That makes it suitable for material you would normally avoid pasting into a hosted tool, such as:

- CloudFormation and Terraform
- Jenkins configuration
- JSON/YAML manifests
- logs and diagnostic output
- test payloads
- URLs, tokens and encoded strings

Important: tools such as JWT Decoder intentionally decode data but **do not verify signatures**. YAML and some language formatters use conservative, best-effort parsers rather than pretending to be complete language implementations.

## Included tools

### Formatters

- JSON Formatter / validator / tree view
- XML Formatter / validator
- HTML Formatter
- CSS Formatter
- JavaScript Formatter
- SQL Formatter

### Minifiers

- CSS Minifier
- JavaScript Minifier

### Escapers

- JSON Escape / Unescape
- XML Escape / Unescape
- HTML Escape / Unescape
- JavaScript Escape / Unescape
- Java / .NET Escape
- CSV Escape / Unescape
- SQL Escape

### Encoders / cryptography

- URL Encoder / Decoder
- Base64 Encoder / Decoder
- SHA-1 / SHA-256 / SHA-384 / SHA-512

### Converters

- JSON -> XML
- XML -> JSON
- JSON -> YAML
- YAML -> JSON (conservative parser)
- CSV -> JSON
- CSV -> XML
- Epoch Timestamp Converter
- JSON Lines / NDJSON

### Validators / inspectors

- Regex Tester
- JWT Decoder
- Query String Parser
- CIDR Calculator
- MIME Type Lookup

### String / web utilities

- String Utilities
- UUID Generator
- HTML Entity / Character Converter

## Running it

Open `index.html` directly in a modern browser.

For GitHub Pages, publish the repository from the root of the default branch. No build process is required.

## Suggested repository structure

```text
local-developer-tools/
  index.html
  README.md
  LICENSE
  SECURITY.md
```

## Contributing

Keep tools dependency-free where practical and avoid network calls. A useful contribution should work offline after the page is loaded.

## Credits / homage

The project is inspired by the classic FreeFormatter developer toolbox and especially its straightforward formatter, escaper and converter pages. The goal is preservation of the *idea and usefulness* of those utilities, not an attempt to impersonate the original service.
