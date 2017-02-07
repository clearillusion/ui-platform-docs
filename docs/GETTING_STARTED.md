Get started with P2 UI Platform using the Angular CLI.

## Install the CLI

```bash
npm install -g @angular/cli@latest
```

## Create a new project

```
ng new my-project
```

The new command creates a project with a build system for your Angular app.

## Install P2 UI Platform Startup module

```bash
npm install --save @p2/startup
## (optional) Additional P2 Platform UI Modules installs
npm install --save @p2/core @p2/ui @p2/styles
```

## Import the P2 UI Platform Startup NgModule

**src/main.ts**
```ts
import './polyfills.ts';
import { platformBrowserDynamic } from '@angular/platform-browser-dynamic';
import { enableProdMode } from '@angular/core';
import { environment } from './environments/environment';
import { PuiStartupModule } from '@p2/startup';
import { AppModule } from './app/';

if (environment.production) {
  enableProdMode();
}

PuiStartupModule.forRoot(AppModule);
platformBrowserDynamic().bootstrapModule(PuiStartupModule);
```
## Bootstrap 
**index.html**
```html
...
<body>
  <pui-app-root>
    <div style="padding: 20%;text-align:center;">
      <h3>P2 Loading...</h3>
    </div>
  </pui-app-root>
</body>
...
```

## Include the core and theme styles
This is **required** to apply all of the core and theme styles to your application.

**angular-cli.json**
```json
{
    ...,
    "apps": [
        ...,
        "styles": [
        "../node_modules/@p2/styles/core.css",
        "styles.css"
        ],
        "scripts": [
            "../node_modules/@p2/styles/core.js"
        ],
        ...
    ],
    ...
}
```

## Sample P2 UI Platform project
- [P2 UI QuickStart](http://ui-quickstart.azurewebsites.net)