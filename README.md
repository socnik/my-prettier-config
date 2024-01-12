# My Prettier Config

[![Prettier Banner](https://raw.githubusercontent.com/prettier/prettier-logo/master/images/prettier-wide-dark.svg)](https://github.com/prettier)

This is my favorite prettier config for my projects.

## Usage

You can see [official Prettier docs](https://prettier.io/docs/en/configuration#sharing-configurations) or follow this steps:

### 1. Install `@socnik/my-prettier-config` package

Npm: `npm i --dev @socnik/my-prettier-config`
Pnpm: `pnpm add -D @socnik/my-prettier-config`

### 2. Add config to your `package.json`

```json
{
  "name": "my-cool-library",
  "version": "9000.0.1",
  "prettier": "@socnik/my-prettier-config" // <- Add this line
}
```

### 3. Enjoy 🚀!

## Config content

Config contents in [`.prettierrc.json`](https://github.com/socnik/my-prettier-config/blob/main/.prettierrc.json) file.

```yaml
arrowParens: always,
bracketSameLine: false,
bracketSpacing: true,
cursorOffset: -1,
embeddedLanguageFormatting: auto,
endOfLine: lf,
htmlWhitespaceSensitivity: "css",
jsxSingleQuote: true,
printWidth: 80,
proseWrap: preserve,
quoteProps: as-needed,
semi: false,
singleAttributePerLine: true,
singleQuote: true,
tabWidth: 2,
useTabs: false,
trailingComma: es5,
vueIndentScriptAndStyle: false
```
