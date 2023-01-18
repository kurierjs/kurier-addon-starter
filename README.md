# kurier-addon-starter

Build your own Kurier addon using this repo as a template!

## Usage

Clone this repo or create a new repo using GitHub's template feature.

## Structure

An addon's minimal structure requires:

- `src/index.ts` - where the addon is exported via `export default`.
- `src/types.ts` - any own type definitions or type extensions from Kurier's base interfaces.
- `src/addon.ts` - the file that contains the class that extends from `Addon`, with an `install()` method that initializes the addon.

## Tooling

This repo has support for TypeScript + ESLint + Prettier, along with `install-peers-cli` to install a version of Kurier alongside your addon.

## Naming the addon

Official addons are registered in the `@kurier` NPM scope. For example:

```
@kurier/addon-transport-layer-context
```

Community addons are named `kurier-addon-*`. For example:

```
kurier-addon-wordbot
```

## Publishing

If you want your addon listed in the Kurier readme and docs, create an issue here, pointing to your repository along with a description of how it works and what it does.
