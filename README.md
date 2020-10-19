### Start
```
npm init
```




### Settings
```
npm install babel-cli
npm install babel-preset-env
npm run build // the ES5 code in ./lib/main.js.
```
 -D flag instructs npm to add each package to a property called devDependencies in package.json. simply run npm install — it instructs npm to look inside package.json and download all of the packages listed in devDependencies
 
 
### Setup

```
./src/main.js
```

### Path

```
project
|_ node_modules
|___ .bin
|___ ...
|_ src
|___ main.js
|_ .babelrc
|_ package.json
```

### babelrc

touch .babelrc
```
{
  "presets": ["env"]
}
```

### package.json

```
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build":"babel src -d lib"
  }
```
```
babel — The Babel command call responsible for transpiling code.
src — Instructs Babel to transpile all JavaScript code inside the src directory.
-d — Instructs Babel to write the transpiled code to a directory.
lib — Babel writes the transpiled code to a directory called lib.
```
