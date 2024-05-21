# My Prettier Config

<a href="https://github.com/prettier">
   <p align="center">
    <img
     src="https://raw.githubusercontent.com/prettier/prettier-logo/master/images/prettier-wide-dark.svg"
     alt="Prettier Banner"
    >
   </p>
</a>

My preferred [Prettier config](https://prettier.io) which i use between my projects.

I recommend using this config with my [Editoconfig template](https://github.com/socnik/my-editorconfig). They are fully compatible between themselves.

This config is in the [`.prettierrc.json`](https://github.com/socnik/my-prettier-config/tree/main/.prettierrc.json) file.

## Usage

### Stage 0

Install `prettier` and `@socnik/my-prettier-config` packages:

```shell
npx nypm add -D prettier @socnik/my-prettier-config
```

### Stage 1

Add config to your `package.json`:

```jsonc
// package.json

{
  "name": "my-cool-library",
  "version": "9000.0.1",
  // ...
  "prettier": "@socnik/my-prettier-config", // <- Add this line
}
```

### Stage 2 _(Optional)_

Install [`Prettier` VSCode extension](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) from marketplace.

### Stage 3

Add your package manager lockfile to `.prettierignore`:

```ignore
# .prettierignore

# Pnpm
pnpm-lock.yaml

# Npm
package-lock.json
```

### Stage 4a _(optional)_

Setup VSCode environment with workspace configuration:

```jsonc
// .vscode/extensions.json

{
  "recommendations": [
    // ...
    "esbenp.prettier-vscode",
    // ...
  ],
}
```

```jsonc
// .vscode/settings.json

{
  // Prettier
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
}
```

### Stage 4b _(optional)_

Setup VSCode environment with [`Devcontainer configuration`](https://code.visualstudio.com/docs/devcontainers/containers):

```jsonc
// .devcontainer/devcontainer.json

{
  // ...
  "customizations": {
    "vscode": {
      "settings": {
        // Prettier
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.formatOnSave": true,
      },
      "extensions": ["esbenp.prettier-vscode"],
    },
  },
}
```

### Stage 5 _(optional)_

Setup Editorconfig with my config. If you want to do it, follow the instructions in [socnik/my-editorconfig](https://github.com/socnik/my-editorconfig#readme) repository.

### Stage 6

Enjoy 🚀!
