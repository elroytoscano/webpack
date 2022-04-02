## HTML, Vanilla JS and Webpack setup

### Features

- Provides support to import/export modules, instead of using `<script type="module"></script>`
- Webpack is used by running `scripts:{ build: "webpack"}`
- Additional options to configure the way webpack should run can be done by changing the `package.json`'s `build` script to `"webpack --mode production"`
- Alternately, a webpack.config.js file can be made as well

### webpack.config.js file properties

- Uses commonjs syntax
  e.g.`module.exports={}`
- For single file entry:
- `entry: path.resolve(__dirname, '/src/index.js'), output: { path: path.resolve(__dirname, 'dist'), filename: 'main.js', },`
- For multiple file entries:
- ` entry: { bundle: path.resolve(__dirname, '/src/index.js'), }, output: { path: path.resolve(__dirname, 'dist'), filename: '[name].js', },`
