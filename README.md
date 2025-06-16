# [Practice] Restaurant Fantasy

![Screenshot of the project](https://github.com/user-attachments/assets/ad5f2819-c958-4f33-81ae-a6174ac1a341)

## Webpack practice

This project was created as practice for some of the basics of using Webpack. For this reason, the focus was on creating modules that inject all the HTML content using JavaScript modules structures (ESM) for the two available sections. Other simple concepts, such as IIFE (Immediately Invoked Function Expressions) and a basic adaptation for responsiveness, were also implemented. However, it was not designed as mobile-first.

## Installation

To run this project locally:

1. **Clone the repository**

```bash
git clone https://github.com/your-username/restaurant-fantasy.git
```

2. **Navigate to the project directory**

```bash
cd restaurant-fantasy
```

3. **Install dependecies**

```bash
npm install
```

4. **Run the development server**

```bash
npx webpack serve
```

## Concepts

### webpack && webpack-CLI

- Module bundler that processes and bundles JavaScript files and optimizes some assets.
- The CLI provides a way to interact with Webpack.

### webpack-dev-server

- Allows to have a live server without creating a fully optimized production build.

### css-loader && style-loader

- The former exports the CSS as a string and converts it into a JavaScript module, while the latter injects those styles into the DOM using `<style>` tags.

### html-webpack-plugin

- Automatically injects the generated JavaScript and CSS files (imported for its side effect in _index.js_) into the HTML.

### webpack-merge

- It's recommended to separate the logic between different environments, such as development and production, as we'll need different configurations for each one, like changing the source mapping. But as the webpack documentation says, "we'll still maintain a 'common' configuration to keep things DRY".
