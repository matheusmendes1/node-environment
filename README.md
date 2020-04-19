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

## Some considerations

## About package.json

* '--transpileOnly': as your project becomes bigger, compilation time increases linearly. It's because typescript's semantic checker has to inspect all files on every rebuild. The simple solution is to disable it by using the transpileOnly: true option, but doing so leaves you without type checking and will not output declaration files.

* '--inspect': possibility of vs code connecting to an application in the development environment

* '--ignore-watch node_modules': will ignore the files in node_modules when it comes to watching files

* Executing "yarn dev: server" will upload the server following the settings of the variable
