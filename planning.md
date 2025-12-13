---
author: bladeacer
last-updated: 03-12-2025
---

#### Focus
Pure SCSS

#### Compilation
Binary calling (install sass and directly call)

JS setup (dotenv related setup)

##### Mix of CSS/SCSS
https://github.com/primary-theme/obsidian/blob/main/Gruntfile.js

https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/.stylelintrc.json

##### Pure SCSS
https://github.com/dbarenholz/halcyon-obsidian/blob/main/package.json

#### Linting
Stylelint > PostCSS > Prettier.
> Functionality over form/aesthetics

You can have both functionality and aesthetics with `stylelint-prettier`, however.

PostCSS mentioned?
> Too opinionated/niche tho

Include stylelint no-unsupported-browser-feature plugin

Both are not really used too often.

#### File structure
`theme.scss` contains all `@use`

`theme.scss` contains some `@use` which calls other `@use`
> CWD + main SCSS file in sub-directory
>
> Can use `some_dir/_index.scss` and have it called as `@use 'some_dir/';`

various `@use` entry points in scss directory.

> Larger codebases generally have dated versions of files scattered across the codebase

Recommend certain file structures, do not really enforce. Let the theme dev decide.

#### Initial Setup helper
E.g. Halcyon/Primary/FAS (not final). Showcase each structure and let users generate base on that with the initial setup.

https://github.com/plopjs

#### SCSS/CSS
Some do pure SCSS output to CSS files others do a mix.

#### Source maps?
Generally no

#### Minification of `theme.css`?
Generally no

#### Issue Templates
Maple theme has some really good defaults

https://github.com/subframe7536/obsidian-theme-maple/tree/1.0/.github/ISSUE_TEMPLATE

#### Version Bump/Other Script?
Depends.

`release.yml` is basically everywhere

Generally no contributing or code-of-conduct related markdown files.

#### Default batteries included snippets
Core slides plugin other niceties with CSS variables I guess

___

Employ sane defaults, let users use plop.js for templating initial setup (set default values).
