# obsi-scss-template

The missing Obsidian SCSS theme template.

## Why I made this

1. Existing theme templates are dated
2. Existing themes assume CSS only, while most larger themes out there make use
of SCSS.
3. Existing theme templates are not opinionated enough

### Why SCSS over CSS
SCSS has *a lot* of niceties over vanilla CSS, such as:

- Strict superset
- Infinite nesting (though it should probably not be abused)
- `@mixin`s (think `Functions` in a traditional programming language)
- `@extends` (reusable code snippets)
- `@use` so you can split and organise your codebase
- Loops, yes. Loops.

And a lot more. You can find out more about it at the [official site](https://sass-lang.com/).

## Usage

### Use as template

Click `Use as template` > `Create a new repository`.

### Understanding the starter codebase

Do take the time to read through this file, the configured Stylelint defaults
and the project structure under the [scss](./scss/) folder.

Each of the files should have comments explaining why they are there and what
they are there for. Feel free to modify or remove defaults you do not like.

### Scripts
This repository comes with some scripts. The important ones include:

- `npm run dev`: SCSS to CSS compiler, assumes you have
[Sass](https://sass-lang.com/) (Dart, Node) installed
- `npm run lint`: Lints the entire SCSS codebase. Reruns linting when a file
write is detected in source files
- `npm run lint-once`: As its namesake says, lints the codebase once
- `npm run fix`: Equivalent to running `stylelint --fix`. Run this only after
your file changes are saved.

## Questions
TBC.

## Status
WIP.

## License

Unlicense, see [LICENSE](./LICENSE).

Note: By contributing code to this project in any form, including sending a pull
request via GitHub, a code fragment or patch via private email or public
discussion groups, you agree to release your code under the terms of the
Unlicense license that you can find [here](./LICENSE).

### Credits

- Primary
- Fancy-a-Story
- Maple
- Minimal
- ITS
- Halcyon
- [Obsidian Theme Template](https://github.com/obsidian-community/obsidian-theme-template)
- [Obsidian Sample Theme](https://github.com/obsidianmd/obsidian-sample-theme)
- ...probably missed a few others
