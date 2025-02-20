# Babel Example

This project demonstrates how to use Babel to transpile modern JavaScript and JSX code into browser-compatible JavaScript.

## Table of Contents

- [Introduction](#introduction)
- [Setup](#setup)
- [Babel Configuration](#babel-configuration)
- [Running the Example](#running-the-example)
- [Customizing the Example](#customizing-the-example)
- [Resources](#resources)
- [License](#license)

## Introduction

Babel is a popular JavaScript compiler that allows you to write modern JavaScript and JSX, and convert it to code that can run in older browsers or environments. This example demonstrates how to set up Babel with `@babel/preset-env` and `@babel/preset-react` to transpile both modern JavaScript and React JSX.

## Setup

To get started with this example, follow these steps:

1. Clone this repository to your local machine:
```
   git clone https://github.com/khachatryan-dev/babel.git
   cd ./babel
```

2. Install the required dependencies:
```
   npm install
```
   or if you're using Yarn:
```
   yarn install
```

## Babel Configuration

The configuration file `babel.config.js` defines the Babel presets for the project. Here’s how the configuration file looks:
```
js

module.exports = {
   presets: ['@babel/preset-env', '@babel/preset-react'],
};
```
- `@babel/preset-env`: Transpiles modern JavaScript code to older versions compatible with older browsers.
- `@babel/preset-react`: Compiles JSX code into standard JavaScript to be used in React applications.

## Running the Example

To run the example code, you can use `babel-node` or Babel CLI.

### Using Babel-Node

To run the example with Babel-Node, use the following command:
```
npx babel-node index.js
```
This will execute the code and print:

Hello, Babel User!


### Using Babel CLI

Alternatively, you can manually compile and run the JavaScript:

1. Install Babel CLI:
```
   npm install --save-dev @babel/cli @babel/core
```

2. Add a build script to your `package.json` file:
```
json

"scripts": {
    "build": "babel index.js --out-file compiled.js"
}
```

3. Run the build script:
```
   npm run build
```
   This will transpile the `index.js` file and generate the `compiled.js` file.


## Customizing the Example

You can easily modify this example by adding more modern JavaScript features or updating the JSX code in `index.js`. Babel will take care of transpiling the code to ensure compatibility with older browsers.

To further customize the example:
- Add additional Babel plugins or presets by updating the `babel.config.js` file.
- Update the `index.js` file to include more complex JavaScript or React components.

## Resources

- [Babel Documentation](https://babeljs.io/docs/en/)
- [Babel GitHub Repository](https://github.com/babel/babel)

## License

This example is open-source and available under the MIT License.
