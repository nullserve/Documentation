# Getting Started

To deploy an application, you should use the CLI which will abstract the API calls away into a command that can easily be run on your local developer machine or on CI/CD.

## Installing the CLI

The CLI is available in [NPM](https://www.npmjs.com/package/@nullserve/cli) and can be used independently or within node.js projects.
To install it, run:

<!-- tabs:start -->

#### ** Yarn **

`yarn add --dev @nullserve/cli`

#### ** Npm **

`npm install --save-dev @nullserve/cli`

<!-- tabs:end -->

to add it to the project's dev dependencies.
This won't increase your bundle size but will allow you to use it locally when developing your project.

Once it's installed, you can use the CLI like this:

<!-- tabs:start -->

#### ** Yarn **

`yarn run nullserve help`

#### ** Npm **

`npx nullserve help`

<!-- tabs:end -->

This will run the `help` command and test that the CLI is installed correctly.
The `help` command will also present you with an up-to-date listing of all of the available commands in the CLI.
