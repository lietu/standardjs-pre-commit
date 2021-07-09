# StandardJS hooks for pre-commit

Hook to run [StandardJS](https://standardjs.com) with [pre-commit](https://pre-commit.com).


## Usage

You can add these to your project's `.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/lietu/standardjs-pre-commit
  rev: 16.0.3
  hooks:
    - id: standard
```


## I need ES features, what should I do?

Basically just follow the StandardJS guides: https://standardjs.com/#how-do-i-use-experimental-javascript-es-next-features

You should have a `package.json` at the root including:

```json
{
    "standard": {
        "parser": "@babel/eslint-parser"
    }
}
```

It also seems you need a `babel.config.json` at the root with e.g. `{}` as the contents.



# Financial support

This project has been made possible thanks to [Cocreators](https://cocreators.ee) and [Lietu](https://lietu.net). You can help us continue our open source work by supporting us on [Buy me a coffee](https://www.buymeacoffee.com/cocreators).

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/cocreators)
