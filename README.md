# MyProject

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.1.3.

## Schematics test

#### Install schematic dependencies and build it
```bash
yarn --cwd libs/schematics-test install && \
yarn --cwd libs/schematics-test build 
```

#### Run the schematic with `ng generate` command
```bash 
ng g ./dist/libs/schematics/collection.json:my-test-schematic --localize.locale=de
```
You should see the following error
```
Unknown option: '--localize.locale'
```
 
 
#### Run the schematic with `schematics` command
```bash 
schematics ./dist/libs/schematics/collection.json:my-test-schematic --localize.locale=de
```

The option is passed to the schematic. You should see the following output
```
My test schematic: {"localize":{"locale":"de"}}

```
