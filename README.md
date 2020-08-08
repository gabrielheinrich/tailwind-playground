# Tailwind Playground

A simple starter template for building a static website with Tailwind CSS.

## Getting Started

### yarn

```bash
yarn # install dependencies
yarn serve # run development server with hot-reloading
yarn build # build for production
```

### npm

```bash
npm install # install dependencies
npm run serve # run development server with hot-reloading
npm run build # build for production
```

## Static Assets

Copy all your images and other static assets into src/assets. Webpack will
automatically bundle them with the production build.

```html
<img src="assets/logo.png" />
```

## Custom Font

First add an @import directive to src/style.css

```css
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;700&display=swap");
```

Then add the font to the tailwind.config.js

```js
module.exports = {
  /* ... */
  theme: {
    fontFamily: {
      sans: ["Montserrat", "sans-serif"],
    },
  },
};
```
