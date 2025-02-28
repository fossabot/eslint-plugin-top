# eslint-plugin-top
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fericcornelissen%2Feslint-plugin-top.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fericcornelissen%2Feslint-plugin-top?ref=badge_shield)


Disallow side effects at the top level of files

## Installation

You'll first need to install [ESLint]:

```shell
npm i eslint --save-dev
```

Next, install `eslint-plugin-top`:

```shell
npm install @ericcornelissen/eslint-plugin-top --save-dev
```

## Usage

Add `top` to the plugins section of your `.eslintrc` configuration file. You can
omit the `eslint-plugin-` prefix:

```json
{
  "plugins": ["@ericcornelissen/top"]
}
```

Then configure the rules you want to use under the rules section.

```json
{
  "rules": {
    "@ericcornelissen/top/no-top-level-variables": 2,
    "@ericcornelissen/top/no-top-level-side-effect": 2
  }
}
```

## Supported Rules

- [`no-top-level-variables`](docs/rules/no-top-level-variables.md)
- [`no-top-level-side-effect`](docs/rules/no-top-level-side-effect.md)

[eslint]: https://eslint.org/


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fericcornelissen%2Feslint-plugin-top.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fericcornelissen%2Feslint-plugin-top?ref=badge_large)