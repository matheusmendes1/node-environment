# node-environment
 A Node environment with some presets

## About

This project was created to facilitate the beginning of the construction of an application in Node. In it, there are settings for ESLint and Prettier, as well as settings for the editor and finally, a setting for the VSCode debugger. I hope it is useful.
Remember: the settings are customizable, and here are some of my choices. You can, at any time, change and do it your way

## Prerequisites

* NodeJS
* VSCode
* EditorConfig extension for VSCode
* ESLint extension for VSCode
* Prettier extension for VSCode
* (Optional) Yarn
* Execute "yarn add" or "npm i" to install dependencies

## Some considerations

###### About package.json

* '--transpileOnly': as your project becomes bigger, compilation time increases linearly. It's because typescript's semantic checker has to inspect all files on every rebuild. The simple solution is to disable it by using the transpileOnly: true option, but doing so leaves you without type checking and will not output declaration files.

* '--inspect': possibility of vs code connecting to an application in the development environment

* '--ignore-watch node_modules': will ignore the files in node_modules when it comes to watching files

* Executing "yarn dev: server" will put the server online following the settings of the variable

###### About prettier.config.js

In the prettier config, we say that we want to use single quotes, we want to use a comma whenever we add new elements, parameters or properties to the JavaScript code. Finally, we want to avoid parentheses whenever possible (useful for arrow functions)

###### About ts.config.json

* outDir will tell you where the files go after being transpiled

* rootDir will tell you where the files come from (which will be transpiled)

* strictPropertyInitialization: ensure non-undefined class properties are initialized in the constructor. This option requires --strictNullChecks be enabled in order to take effect.

* experimentalDecorators and emitDecoratorsMetadata will enable decorators for our project. It is useful when creating models, for example.

## Credits and sources

* I learned and learn a lot with the [Rocketseat Team](https://rocketseat.com.br/)

* [Typescript Reference](https://www.typescriptlang.org/docs/handbook/compiler-options.html)

* [ Mozilla developer Refence](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Trailing_commas)
