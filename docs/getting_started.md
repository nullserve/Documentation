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

## Logging in to NullServe

To use NullServe, you need to have a [Github](https://github.com) account.
Go to the [NullServe Console](https://app.nullserve.com) and log in with your Github credentials.

## Creating an API token

An API Token is needed to deploy using the NullServe CLI;
Create an API Token by going to [user settings](https://app.nullserve.com/dashboard/settings).
Note that the API Token name is only used for management convenience so the tokens may be revoked correctly.
Once you create a token, ensure that you copy and save the value, it won't be shown again.
Treat this token like a password, as it allows any person who has it to deploy a site to your account.
Do not check it in to source control or share it with anyone.

## Creating a Site

A site can be created in the web app.

## Deploying a Site with the CLI

A site can be deployed using the CLI with the `deploy` command.

<!-- tabs:start -->

#### ** Yarn **

```shell
export NULLSERVE_API_TOKEN=aBcd3...
yarn run nullserve deploy ./public
```

#### ** Npm **

```shell
export NULLSERVE_API_TOKEN=aBcd3...
npx nullserve deploy ./public
```

<!-- tabs:end -->
