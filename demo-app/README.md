# DemoApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.0.

## First step

Inside the project folder you will need to install all the Node dependencies. You can do this at the command line.
- Ok, so you have a new folder. Open a terminal window or if you are on Windows you have PowerShell. You hold `shift + right click` and in the menu you will see "Open with PowerShell".
- You are now at the command line
- You need to install Angular CLI (command line interface) so you will type `npm install -g @angular/cli`
- We will need to install all the dependencies by typing in `npm install` and it will take a few moments for it to get everything it needs.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

Run `ng serve --open` does the same as above and it automatically opens a browser for you.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.


## Overview

  

The vast majority of the modules you will need are included and placed in a TypeScript file called `material.ts` inside the `src/` folder.

  

  

Like mentioned above, the `src/` folder contains most of the Angular Material components imported, but NOT used in any context yet. You can go to the [Angular Material](https://material.angular.io/components/categories) homepage and get copy-and-paste examples of the components. To see what items are available, you can open the `material.ts` file and see the names of the modules that are imported.

  
### What you get
This is pretty minimal, but it should help. 
- I have the majority of Angular Material components readily available for you to use. Just copy-paste them from [Angular Material](https://material.angular.io/components/categories).
- I use the default indigo-pink Material theme in `styles.scss` but you can change it later.
- I have included Material Icons by linking from `index.html`
- I have created a header and footer and used Material Design's `<mat-card>` wrapping a piece of text to let you know they are working.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).