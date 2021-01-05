# Learning Angular

Angular is a mobile and web development framework that works in the front end.

## Setup
The first step is to install the angular comand line interface.
>$ npm i -g @angular/cli

To create a new angular app,
>$ ng new <app-name>

To run the app, within the angular app, use the following command,
>$ ng serve

This will compile the code within the folder and run the app. Within the terminal, there should be an output with the port that it is running on. The default is `http://localhost:4200/`.

Next, is to install typsecript.
>$ npm install -g typescript

### For learning typescript
You can create a new file called `<new-file>.ts`. This is a typescript file that will need to be transpiled into js. To do this, from within the terminal `$ tsc <new-file>.ts`. This will create a js copy within the same folder as `<new-file>.js`.

For angular projects, `ng serve` will transpile the code under the hood, so you dont have too.

## Breakdown of folder components
The initial creation of an angular app will yeild many folders and files.

- e2e: Stands for end to end. This is where the testing scripts will be stored which can simulate users.

- node-modules: third party libraries are stored in here. This file is NOT deployed, it is for development purposes only.

- src: This is the source code for our app. 
    - app: folder which will contain at least one module, and one component.
    - assets: image and text files
    - environments: this will store the development environment and deployment environment variables.
    - favicon.ico: icon which will be displayed in the browser tab
    - index.html: the html page
    - main.ts: type script file which is the starting point of the application
    - polyfill.ts: contains scripts necessary to allow the app to work on some browsers
    - styles.css: style sheet
    - test.ts: used to set up testing environment

- .gitingore: excludes files when uploading to repository to prevent clutter or leak of information

- angular.json: configuration defaults for build

- karma.config.js: karma is a test runner for javascript

- package.json: contains the name of the dependencies for our app

- tsconfig: type script configuration. 

- tslint.json: static analysis tool for typescript code. Checkes typescript code for readability, maintainability, and functionality errors



