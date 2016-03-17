# No Maintenance Intended

[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)

<img src='https://media.giphy.com/media/h9hoPqk7Db5fi/giphy.gif' height='200'>

This project is no longer actively maintained. It does its job, but there are no plans to extend or change it.
We suggest you to check out [`react-transform-boilerplate`](https://github.com/gaearon/react-transform-boilerplate).

---

What's included:

- Tasks scripts using `npm run`
- [Babel](babeljs.io) compiler ES6 to ES5
- [ES6 lint](http://eslint.org/), [babel-eslint](https://github.com/babel/babel-eslint) and [eslint-plugin-react](https://github.com/yannickcr/eslint-plugin-react)
- CSS support via [style-loder](https://github.com/webpack/style-loader) and [css-loader](https://github.com/webpack/css-loader)
- SVG, PNG, JPG, GIF and fonts via [url-loader](https://github.com/webpack/url-loader)

## Installation

```
npm install
npm run build
```

This package is also on NPM `npm i webpack-react-starter`.

## Development

### Tasks

- `npm run build`
- `npm run examples`
- `npm run lint`

### File Structure

#### dist

The compiled and minified version for distribution generated by `npm run build`.

#### examples

Create your app and demonstrate how the components works. The `npm run examples` starts the [webpack-dev-server](http://webpack.github.io/docs/webpack-dev-server.html) in hot mode.

#### scripts

Bash scripts to perform the build operation.

#### src

Source of the project. Since we're keeping the stylesheet together with the component, have a folder for each one make sense e.g.

```
|-- src
  |-- Menu
    |-- index.js
    |-- index.css
  |-- SearchField
    |-- index.js
    |-- index.css
  |-- index.js
```

#### src/index.js

The `./src/index.js` is the main entry point. Use it to export your modules.

```javascript
export {default as HelloWorld} from './HelloWorld';
```
