<p align="center">
    <img alt="Random Name Picker for Lucky Draw" src="./logo.svg" width="100" />
</p>
<h1 align="center">Random Name Picker for Lucky Draw</h1>

### Configure
To Configure API End Points:
* Go to App.ts and change the api url and the Basic Auth key
* Go to Csp.pug and include the Url Provider in connectSrc and defaultSrc in order to be allowed through


### Technology Stack
* Pug
* CSS3 (SCSS)
* Web Animations API
* AudioContext API

## Development

### Prerequisite
* Node 18 above or nvm installed
* Yarn or NPM installed

### Install dependencies
To install dependencies:
```bash
yarn install
```

### Start development server
To start the development server:
```bash
yarn start
```

### Build production
To build the project for production:
```bash
yarn build
```
All the build files can be found in `/dist` folder.

## General Guidance on Deployment

This app works fine under common static web hosting choices. Here's a general outline of the steps you can follow:

1. Set up your CI/CD pipeline to use Node.js and arn images. (If you prefer not to use a CI/CD pipeline, make sure you have both Node.js and Yarn installed on your machine.)

2. Start by installing the project dependencies. Run the command `yarn install` to ensure that all the necessary npm packages are installed and ready for the build process. To optimize costs and improve the efficiency of your CI/CD pipeline, you can consider adding a cache for the `node_modules` directory. Check your specific CI/CD tool's documentation for cache configuration options.

3. Next, you'll need to build the project. Use the command `yarn build` to initiate the build process. This command will compile and bundle the source code, generating the assets required for hosting.

4. Once the build process is complete, you'll need to copy all the generated assets located under the `/dist` directory. The specific command to accomplish this may vary depending on the CI/CD tool and OS you're using. Typically, you'll need to include a step in your pipeline that copies the contents of the `/dist` directory to a storage accessible by your chosen static web hosting service.
