 <div align="center">
 <img align="center" width="180" src="https://i.imgur.com/62VsVXD.png" />
  <h2>Javascript Library Boilerplate</h2>
  <blockquote>Library Starter Kit for your Javascript projects</blockquote>
  <a href="https://github.com/hodgef/js-library-boilerplate/actions"><img alt="Build Status" src="https://github.com/hodgef/js-library-boilerplate/workflows/Build/badge.svg?color=green" /></a> <a href="https://github.com/hodgef/js-library-boilerplate/actions"> <img alt="Publish Status" src="https://github.com/hodgef/js-library-boilerplate/workflows/Publish/badge.svg?color=green" /></a> <img src="https://img.shields.io/david/hodgef/js-library-boilerplate.svg" /> <a href="https://david-dm.org/hodgef/js-library-boilerplate?type=dev"><img src="https://img.shields.io/david/dev/hodgef/js-library-boilerplate.svg" /></a> <img src="https://api.dependabot.com/badges/status?host=github&repo=hodgef/js-library-boilerplate" />

<strong>This is a more robust library boilerplate. For a minimal alternative, check out [js-library-boilerplate-basic](https://github.com/hodgef/js-library-boilerplate-basic).</strong>
</div>


## ⭐️ Features

- Webpack 4
- Babel 7
- Hot Reloading (`npm start`)
- CSS Autoprefixer
- SASS/SCSS support
- UMD exports, so your library works everywhere.
- Based on [CRA v3.4.1](https://github.com/facebook/create-react-app/releases/tag/v3.4.1) (For Vanilla JS libs or React libs)
- Jest unit testing
- `npm run demo` To build a ready-for-deployment demo [(Example)](https://github.com/hodgef/js-library-boilerplate/tree/master/demo)
- Customizable file headers for your build [(Example 1)](https://github.com/hodgef/js-library-boilerplate/blob/master/build/index.js) [(Example2)](https://github.com/hodgef/js-library-boilerplate/blob/master/build/index.css)
- Configurable `postinstall` message [(Example)](https://github.com/hodgef/js-library-boilerplate/blob/master/bin/postinstall)
- Daily [dependabot](https://dependabot.com) dependency updates

## 📦 Getting Started

```
git clone https://github.com/Zodaka/js-library-boilerplate.git myLibrary
npm install
```

## 💎 Customization

> Before shipping, make sure to:
1. Edit `LICENSE` file
2. Edit `package.json` information (These will be used to generate the headers for your built files)
3. Edit `library: "MyLibrary"` with your library's export name in `./config/webpack.config.js`
4. Edit `./bin/postinstall` (If you would like to display a message on package install)

## 🚀 Deployment
1. `npm publish`
2. Your users can include your library as usual

### npm
```
import MyLibrary from 'my-library';
import 'my-library/build/index.css' // If you import a css file in your library

let libraryInstance = new MyLibrary();
...
```

### self-host/cdn
```
<link href="build/index.css" rel="stylesheet">
<script src="build/index.js"></script>

let MyLibrary = window.MyLibrary.default;
let libraryInstance = new MyLibrary();
...
```