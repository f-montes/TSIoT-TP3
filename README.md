# TSIoT-TP3
Trabajo Practico Testing BDD - CEIoT

Gestion de las parejas en la lista

npm init

npm install --save @cucumber/cucumber chai nyc

gitignore
  node_modules
  coverage
  .nyc_output
  .vscode

Editar el Package.json para:
  {
  "name": "lista-bdd",
  "version": "1.0.0",
  "main": "index.js",
  "scripts": {
    "test": "cucumber-js --publish-quiet",
    "coverage": "nyc --reporter=html cucumber-js --publish-quiet"
  },
  "nyc": {
    "exclude": "features/**"
  },
  "author": "",
  "license": "ISC",
  "dependencies": {
    "@cucumber/cucumber": "^7.3.0",
    "chai": "^4.3.4",
    "nyc": "^15.1.0"
  },
  "devDependencies": {},
  "description": ""
}
