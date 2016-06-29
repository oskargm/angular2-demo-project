# Angular 2

Seguirem el tutorial d'Angular2 que hi ha a la seva web:
    https://angular.io/docs/ts/latest/quickstart.html

Per defecte Cloud9 utilitza node v4.4.5 i npm v2.15.5, cal pujar la versió.
Com utilitzem nvm podem fer:

```
nvm install 6
```

ens baixa la darrera versió 6 i ens quedem amb `node v6.2.2` i `npm v3.9.5`.

Creem el `package.json` amb el contingut per la demo:

```
{
  "name": "angular2-demo",
  "version": "1.0.0",
  "scripts": {
    "start": "tsc && concurrently \"npm run tsc:w\" \"npm run lite\" ",
    "lite": "lite-server",
    "postinstall": "typings install",
    "tsc": "tsc",
    "tsc:w": "tsc -w",
    "typings": "typings"
  },
  "license": "ISC",
  "dependencies": {
    "@angular/common":  "2.0.0-rc.3",
    "@angular/compiler":  "2.0.0-rc.3",
    "@angular/core":  "2.0.0-rc.3",
    "@angular/forms": "0.1.1",
    "@angular/http":  "2.0.0-rc.3",
    "@angular/platform-browser":  "2.0.0-rc.3",
    "@angular/platform-browser-dynamic":  "2.0.0-rc.3",
    "@angular/router":  "3.0.0-alpha.7",
    "@angular/router-deprecated":  "2.0.0-rc.2",
    "@angular/upgrade":  "2.0.0-rc.3",
    "systemjs": "0.19.27",
    "core-js": "^2.4.0",
    "reflect-metadata": "^0.1.3",
    "rxjs": "5.0.0-beta.6",
    "zone.js": "^0.6.12",
    "angular2-in-memory-web-api": "0.0.12",
    "bootstrap": "^3.3.6"
  },
  "devDependencies": {
    "concurrently": "^2.0.0",
    "lite-server": "^2.2.0",
    "typescript": "^1.8.10",
    "typings":"^1.0.4"
  }
}
```

Ara ja podem fer un `npm install` i ho instal·larà tot.

Crearem una carpeta `app` que representa la nostra aplicació i que la cridarem
des de la pàgina html.
