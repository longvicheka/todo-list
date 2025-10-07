<div align="center">

# todolist (Ionic Angular)

A starter Ionic Angular app using standalone components and Capacitor. It includes a basic Home page and routing scaffold. The app name and web output directory are configured for Capacitor and Ionic tooling.

[![last commit](https://img.shields.io/github/last-commit/longvicheka/todo-list)](https://github.com/longvicheka/todo-list/commits)
[![typescript 57.9%](https://img.shields.io/badge/typescript-57.9%25-3178C6?logo=typescript)](https://github.com/longvicheka/todo-list/search?l=typescript)
[![languages 3](https://img.shields.io/github/languages/count/longvicheka/todo-list?style=flat)](https://github.com/longvicheka/todo-list)

![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript)
</div>

## Tech stack

- Angular 18 with standalone APIs.
- Ionic Framework 8 UI components.
- Capacitor 6 for native builds.
- Karma + Jasmine for tests.

## Getting started

Install dependencies with your preferred package manager. Then run the dev server.
```packagemanagers
{
  "commands": {
    "npm": "npm install",
    "yarn": "yarn install",
    "pnpm": "pnpm install",
    "bun": "bun install"
  }
}
```
```bash
# install deps
npm install

# start dev server at http://localhost:4200
npm start
```
## **Available npm scripts**
These scripts are defined in package.json.
* npm start: Run the dev server.
* npm run build: Build the web app to www.
* npm test: Run unit tests.
* npm run lint: Lint the project.
* npm run watch: Rebuild on changes.

## **Project Structure**
Key files and folders found in src and config files:
* src/app/app.routes.ts: Routes for Home and default redirect.
* src/app/home/*: Standalone HomePage component.
* src/main.ts: Bootstraps AppComponent with Ionic and Router.
* src/global.scss: Global Ionic styles imports.
* src/environments/: Dev and prod environment files.
* angular.json: Build, serve, and test configuration.
* ionic.config.json: Ionic project metadata.
* capacitor.config.ts: Capacitor appId, appName, webDir.
* .browserslistrc: Target browser support.

## **Development notes**
* .browserslistrc: Target browser support.
* Default route redirects to /home .
* Global Ionic styles are imported once in src/global.scss .

## **Build**
The production build outputs to www. The prod environment replaces environment.ts via angular.json file replacements .
```bash
1 npm run build
```

## **Capacitor (iOS/Android)**
The production build outputs to www. The prod environment replaces environment.ts via angular.json file replacements .
```bash
1 # add a platform
2 npx cap add ios
3 npx cap add android
4
5 # sync after each build
npx cap sync
```
Open native IDEs:
```bash
1 npx cap open ios
2 npx can open android
```
## **Testing**
Run unit tests with Karma and Jasmine. The Karma configuration and Chrome launcher are present in the repo .
```bash
1 npm test
```
## **Linting**
Run ESLint rules tailored for Angular and templates. Rules live in .eslintrc.json .
```bash
1 npm run lint
```
## **Browser Support**
Targets modern browsers per .browserslistrc .
