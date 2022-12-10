[![Facebook](https://img.shields.io/badge/Facebook-%231877F2.svg?logo=Facebook&logoColor=white)](https://facebook.com/smhabibjr) 
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/smhabibjr) 
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?logo=YouTube&logoColor=white)](https://youtube.com/c/HabibJr)
[![Medium](https://img.shields.io/badge/Medium-12100E?logo=medium&logoColor=white)](https://medium.com/@smhabibjr)

## Table of Contents

- [Update Node](#update-node)
- [VS Code Editor Setup](#vs-code-editor-setup)
- [Linting Setup](#linting-setup)

- [Global Object & Module System](#global-object-and-module-system)
- [__dirname & __filename](#linting-setup)
- [Module System](#linting-setup)
- [Module Wrapper Function](#linting-setup)
- [window vs global Object](#linting-setup)
- [window vs global Object](#linting-setup)
- [window vs global Object](#linting-setup)
- [Contact](#contact)

<!-- UPDATE NODE -->

## Update Node

Please follow the below instructions to update node in your machine:

### Windows

1. Update npm
   ```sh
   npm install npm@latest -g
   ```
2. Clear npm cache
   ```sh
   npm cache clean -f
   ```
3. Install n
   ```sh
   npm install -g n
   ```
4. Update node to latest version
   ```sh
   n latest
   ```

<!-- INSTALL & UPDATE YARN -->

## Install and Update yarn

Please follow the below instructions to install or update yarn in your machine.

### On Windows

1. Install yarn
   ```sh
   npm install -g yarn
   ```
2. Update yarn
   ```sh
   yarn set version latest
   ```

### On Mac

1. Install yarn
   ```sh
   brew install yarn
   ```
2. Update yarn
   ```sh
   brew update
   brew upgrade yarn
   ```

<!-- EDITOR SETUP -->

## VS Code Editor Setup

In order to follow along the tutorial series, I recommend you to use Visual Studio Code Editor and install & apply the below extensions and settings.

### Extensions

Install the below extensions:

- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Path Autocomplete](https://marketplace.visualstudio.com/items?itemName=ionutvmi.path-autocomplete)

### Settings

Go to your Visual Stuido Code `settings.json` file and add the below settings there:

```json
// config related to code formatting
"editor.defaultFormatter": "esbenp.prettier-vscode",
"editor.formatOnSave": true,
"[javascript]": {
  "editor.formatOnSave": false,
  "editor.defaultFormatter": null
},
"editor.codeActionsOnSave": {
  "source.fixAll.eslint": true,
  "source.organizeImports": true
},
"eslint.alwaysShowStatus": true
```

### Set Line Breaks

Make sure in your VS Code Editor, "LF" is selected as line feed instead of CRLF (Carriage return and line feed). To do that, just click LF/CRLF in bottom right corner of editor, click it and change it to "LF". If you dont do that, you will get errors in my setup.

![image](https://user-images.githubusercontent.com/77357735/204080659-3aaddc90-4da2-4c94-8e75-96a6c49ad2a8.png)

<!-- LINTING SETUP -->

## Linting Setup

In order to lint and format your code automatically according to popular airbnb style guide, I recommend you to follow the instructions as described in video. References are as below.

### Install Dev Dependencies

```sh
yarn add -D eslint prettier
npx install-peerdeps --dev eslint-config-airbnb-base
yarn add -D eslint-config-prettier eslint-plugin-prettier
```

### Setup Linting Configuration file

Create a `.eslintrc.json` file in the project root and enter the below contents:

```json
{
  "extends": ["prettier", "airbnb-base"],
  "parserOptions": {
    "ecmaVersion": 12
  },
  "env": {
    "commonjs": true,
    "node": true
  },
  "rules": {
    "no-console": 0,
    "indent": 0,
    "linebreak-style": 0,
    "prettier/prettier": [
      "error",
      {
        "trailingComma": "es5",
        "singleQuote": true,
        "printWidth": 100,
        "tabWidth": 4,
        "semi": true
      }
    ]
  },
  "plugins": ["prettier"]
}
```

### Global Object and Module System

As we know that in vanilla javascript we can find window objects in the browser. Inside the window object, we can find lots of built-in functions such as SetTimeout, SetInterval, alert, onClick, and so on. But in node.js we don't have a window object. But still, SetTimeout or SetInterval function works on node.js then questions rising how it works actually.

Well, in node.js we don't have any windows object instead we have a Global object. To see it write console.log(global) we will find some built-in functions inside the global object.

## Contact

<sup align="right"><a href="#table-of-contents">Go to top</a></sup>
