# MonoWorkspace

this project was created by monorepo arquitecture

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 15.2.9.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

## Command Reference

ng new mono-workspace --create-application=false
cd mono-workspace
ng g application host-app --routing --style=scss
ng g application mfe-app --routing --style=scss
ng s host-app -o
ng s mfe-app -o --port 4300
npm i webpack webpack-cli --save-dev
ng add @angular-architects/module-federation --project host-app --port 4200
ng add @angular-architects/module-federation --project mfe-app --port 4300

After configuring module federation in mfe-app, run:
ng s mfe-app -o

ng g c home --project=host-app
ng g c todo --project=host-app

ng g module todo-list --project=mfe-app
ng g c todo-list --project=mfe-app


http://localhost:4300/remoteEntry.js -> Watch the generated MFE webpack
