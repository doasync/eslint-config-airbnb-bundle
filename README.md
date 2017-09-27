# Eslint with Airbnb style

![ESLint Airbnb Standard JS logo](https://i.imgur.com/vPaV2CK.png?1)

ESLint bundled with the original Airbnb Style config. Global installation!

See [airbnb/javascript] for more information. [Compare] configs.

[airbnb/javascript]: https://github.com/airbnb/javascript
[Compare]: https://npmcompare.com/compare/eslint-config-airbnb,standard

## Installation

Install it globally:

```bash
npm install --global eslint-config-airbnb-bundle
```

You can install it locally as well:

```bash
npm install --save-dev eslint-config-airbnb-bundle
```

## Usage

You can now run feature packed `eslint` from any directory:

```bash
eslint -v
```

Create `.eslintrc` file in your project. Setup your IDE / Editor. And be smart!

ES6, ES7, React, JSX, async/await - all new features supported by default 👍

## Sublime Text 3

1. Install this package globally

2. Go to: *Preferences -> Package Control -> install package*

3. Install [SublimeLinter](https://packagecontrol.io/packages/SublimeLinter)

4. Install [SublimeLinter-contrib-eslint](https://packagecontrol.io/packages/SublimeLinter-contrib-eslint)

5. Run:
    ```bash
    npm bin -g
    ```
    ... and copy the path
6. Go to: *Tools -> SublimeLinter -> Open User Settings*

   Paste the path to NodeJS installation folder inside "paths" for your OS and save:
    ```json
    "paths": {
        "linux": [
            "~/.nvm/versions/node/v8.5.0/bin"
        ],
        "osx": [],
        "windows": ["%AppData%\\npm"]
    },
    ```
7. Create `.eslintrc` file inside your working project:
    ```json
    {
      "extends": ["airbnb-bundle"]
    }
    ```

8. Restart Sublime Text

9. Go to *Tools -> SublimeLinter -> Lint this view*

10. You can switch to squiggly underline mark style from *Tools*. Have fun!

![Example](http://i.imgur.com/3nzwkdK.png?1)

## WebStorm

File ➤ Settings / Default Settings ➤ Languages and Frameworks ➤ JavaScript ➤ Code Quality Tools ➤ ESLint

![ESLint settings](http://i.imgur.com/ZznYeJU.png)

Global installation in not necessary for WebStorm, but it is handy for the "Default Settings".

## Custom Config

Add your own rules to the `.eslintrc` file in your project folder.

