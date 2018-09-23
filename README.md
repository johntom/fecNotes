# fecNotes
## How to add a plugin
nvm use 9.11.2
1. au new (take all defaults) or clone AUClean, AUCleanBase01292018
2. au install aurelia-dialog or desired component
3. modify C:\Frameworks\Frontend\AUClean3\aurelia_project\aurelia.json 
adding the following
{
"name": "aurelia-dialog",
"main": "aurelia-dialog",
"path": "../node_modules/aurelia-dialog/dist/amd",
"resources": []
}

		  
{
  "name": "AUClean",
  "type": "project:application",
  "bundler": {
    "id": "cli",
    "displayName": "Aurelia-CLI"
  },
  "build": {
    "targets": [
      {
        "id": "web",
        "displayName": "Web",
        "index": "index.html",
        "baseDir": ".",
        "output": "scripts"
      }
    ],
    "options": {
      "minify": "stage & prod",
      "sourcemaps": "dev & stage"
    },
    "bundles": [
      {
        "name": "app-bundle.js",
        "source": [
          "[**/*.js]",
          "**/*.{css,html}"
        ]
      },
      
      {
        "name": "vendor-bundle.js",
        "prepend": [
          "node_modules/bluebird/js/browser/bluebird.core.js",
          {
            "path": "node_modules/aurelia-cli/lib/resources/scripts/configure-bluebird-no-long-stacktraces.js",
            "env": "stage & prod"
          },
          {
            "path": "node_modules/aurelia-cli/lib/resources/scripts/configure-bluebird.js",
            "env": "dev"
          },
          "node_modules/requirejs/require.js"
        ],
        "dependencies": [
          "aurelia-binding",
          "aurelia-bootstrapper",
          "aurelia-dependency-injection",
          "aurelia-event-aggregator",
          "aurelia-framework",
          "aurelia-history",
          "aurelia-history-browser",
          "aurelia-loader",
          "aurelia-loader-default",
          "aurelia-logging",
          "aurelia-logging-console",
          "aurelia-metadata",
          "aurelia-pal",
          "aurelia-pal-browser",
          "aurelia-path",
          "aurelia-polyfills",
          "aurelia-route-recognizer",
          "aurelia-router",
          "aurelia-task-queue",
          "aurelia-templating",
          "aurelia-templating-binding",
          {
            "name": "aurelia-templating-resources",
            "path": "../node_modules/aurelia-templating-resources/dist/amd",
            "main": "aurelia-templating-resources"
          },
          {
            "name": "aurelia-templating-router",
            "path": "../node_modules/aurelia-templating-router/dist/amd",
            "main": "aurelia-templating-router"
          },
          {
            "name": "aurelia-testing",
            "path": "../node_modules/aurelia-testing/dist/amd",
            "main": "aurelia-testing",
            "env": "dev"
          },
          "text",
          {
            "name": "aurelia-dialog",
            "main": "aurelia-dialog",
            "path": "../node_modules/aurelia-dialog/dist/amd",
            "resources": []
          }
        ]
      }
     
    ],
    
    "loader": {
      "type": "require",
      "configTarget": "vendor-bundle.js",
      "includeBundleMetadataInConfig": "auto",
      "plugins": [
        {
          "name": "text",
          "extensions": [
            ".html",
            ".css"
          ],
          "stub": true
        }
      ]
    }
  },
  "platform": {
    "id": "web",
    "displayName": "Web",
    "index": "index.html",
    "baseDir": ".",
    "output": "scripts"
  },
  "transpiler": {
    "id": "babel",
    "displayName": "Babel",
    "fileExtension": ".js",
    "options": {
      "plugins": [
        "transform-es2015-modules-amd"
      ]
    },
    "source": "src/**/*.js"
  },
  "markupProcessor": {
    "id": "minimum",
    "displayName": "Minimal Minification",
    "fileExtension": ".html",
    "source": "src/**/*.html"
  },
  "cssProcessor": {
    "id": "none",
    "displayName": "None",
    "fileExtension": ".css",
    "source": "src/**/*.css"
  },
  "editor": {
    "id": "vscode",
    "displayName": "Visual Studio Code"
  },
  "unitTestRunner": {
    "id": "karma",
    "displayName": "Karma",
    "source": "test/unit/**/*.js"
  },
  "paths": {
    "root": "src",
    "resources": "resources",
    "elements": "resources/elements",
    "attributes": "resources/attributes",
    "valueConverters": "resources/value-converters",
    "bindingBehaviors": "resources/binding-behaviors"
  },
  "testFramework": {
    "id": "jasmine",
    "displayName": "Jasmine"
  }
}

3. au build - this will generate C:\Frameworks\Frontend\AUClean3\scripts\aurelia-dialog.js
4. create a new account in FEC i called it bundles
5. create a directoru called aurelia-dialog
6. copy  file created in step 3 aurelia-dialog.js to bundles\aurelia-dialog
7. add     "aurelia-dialog": "http://5924b98cbd966f546312882f.blob.core.windows.net/bundles/aurelia-dialog/aurelia-dialog"
      to paths
	  <!doctype html>
<html>
  <head>
    <title class="drag-container drag-item">Sample Layout</title>
    <meta charset="utf-8" class="drag-item">
    <meta http-equiv="X-UA-Compatible" content="IE=edge" class="drag-item">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" class="drag-item">
    <style>
      html, body {
        height: 100%;
      }
      .loading {
        position: absolute;
        top: 50%;
        left: 50%;
        margin-left: -100px;
      }
    </style>    
    <link rel="shortcut icon" href="http://frontendcreator.com/favicon.ico" type="image/x-icon" class="drag-item">
    <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1q8mTJOASx8j1Au+a5WDVnPi2lkFfwwEAa8hDDdjZlpLegxhjVME1fgjWPGmkzs7" crossorigin="anonymous" class="drag-item">
    <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet" class="drag-item">
    <link rel="stylesheet" href="https://kendo.cdn.telerik.com/2017.2.621/styles/kendo.common.min.css" class="drag-item">
    <link rel="stylesheet" href="https://kendo.cdn.telerik.com/2017.2.621/styles/kendo.default.min.css" class="drag-item">
    <link rel="stylesheet" href="https://kendo.cdn.telerik.com/2017.2.621/styles/kendo.bootstrap.min.css" class="drag-item">
    </head>
  <body aurelia-app="src/main">
    <h1 class="loading">Loading...</h1>    
    
    <script src="https://mattduffield.github.io/rjs-bundle/node_modules/requirejs/require.js" class="drag-container drag-item"></script>
    <script src="https://mattduffield.github.io/rjs-bundle/config.js" class="drag-container drag-item"></script>
    <script class="drag-container drag-item">
      require.config({
        paths: {     
             "moment": "https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.18.1/moment.min",
          "jquery": "https://code.jquery.com/jquery-3.1.1.min",
          "bootstrap": "https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min",
          "aurelia-fetch-client": "https://mattduffield.github.io/rjs-bundle/node_modules/aurelia-fetch-client/dist/amd/aurelia-fetch-client",
          "kendo.all.min": "https://fec.blob.core.windows.net/bundles/kendo-ui/2017.2.621/kendoui-javascript",
          "aurelia-kendoui-bridge": "https://fec.blob.core.windows.net/bundles/kendo-ui/2017.2.621/aurelia-kendoui-bridge",
          "aurelia-dialog": "http://5924b98cbd966f546312882f.blob.core.windows.net/bundles/aurelia-dialog/aurelia-dialog"
          
        },
        shim: {
          'bootstrap': ['jquery']
        }
      })
    </script>
    <script src="https://mattduffield.github.io/rjs-bundle/bundles/aurelia.js" class="drag-container drag-item"></script>
    <script src="https://mattduffield.github.io/rjs-bundle/bundles/babel.js" class="drag-container drag-item"></script>
    <script class="drag-container drag-item">
      require(['aurelia-bootstrapper']);
    </script>
  </body>
</html>