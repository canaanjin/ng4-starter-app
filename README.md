# ng2-starter-app

An easy way to get started with an Angular2 application.

Demonstrates
* Simple Hello World! Application that can be easily customized
* AOT compilation for building applications in a production environment
* JIT compilation with SystemJS for rapid development
* Bundling, Compression, and Minification
* Export to multiple module formats: UMD, AMD, and CJS.

## Installation
Install the starter application from npm: 

`npm install ng2-starter-app`

## Usage
You can build the application in three modes: 
* Development
* Production
* Feature Module

# Build Targets
## Development
`gulp dev`
 
 Compiles the application to CommonJS module format and deploys the generated Js files to the `src` folder.

## Production
`gulp app`

Compiles the application, inlines the HTML templates, and creates three static bundles in the `dist` folder:

* app.bundle.js  (contains the application-specific code)
* vendor.bundle.js (contains the vendor-specific libraries - i.e. zone.js, core-js)
* styles.bundle.js (contains the CSS stylesheets)

## Feature Module 
`gulp module`

Compiles the application and deploys the generated Js files to the `dist\src` folder.  
Three bundles under the `dist` folder target various module formats:
* package.bundle.umd.js / package.bundle.umd.min.js
* package.bundle.cjs.js / package.bundle.cjs.min.js
* package.bundle.amd.js / package.bundle.amd.min.js

The bundles exclude external vendor libraries (i.e. @angular or rxjs)

# Script Targets
## Build
* `npm run app` - Builds the application for production and launches a browser window.
* `npm run dev` - Builds the application for development and launches a browser window.
* `npm run build-app` - Builds the application for production.
* `npm run build-dev` - Builds the application for development.
* `npm run serve-app` - Launches a browser window and serves the application for production.
* `npm run serve-dev` - Launches a browser window and serves the application for development.
