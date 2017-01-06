# WebIDE-Frontend

This repo contains frontend code of the Coding WebIDE Community Edition. Please refer to the [WebIDE](https://github.com/pixelorz/webide) repo for instruction on running the whole project.

## Requirement

The repo is written in ES2015, to avoid complications once and for all, please make sure your environment have the right version of node. We use:

- node **v6.x**
- yarn

We strongly recommend `yarn` as your package manager, it will certainly save you from lots of npm induced headache ;-) If you don't have `yarn` installed yet, install it globally by running.
```
npm install yarn -g
```
To learn more about `yarn`, check out their [official site](https://yarnpkg.com/).

By design a "WebIDE" is supposed to run on a _server_ and accessed by web, thus a unix-like environment is strongly recommended. Support for Windows platform will come eventually, but presumably it'll always be lagging behind.

## Development

To start development on this repo, run:
```
yarn
yarn start
```

If you insist that you don't want yarn, well, you can still run:
```
npm install
npm start
```

If ever encountered any problem, double check to ensure your node version is at v6.x with `node -v`, and re-run `yarn`(`npm install`) to update dependencies before you report any issue.


## Configuration

By default the backend host that this frontend connects to is `http://localhost:8080`, this can be changed in `app/config.js`. `webpack-dev-server` by default serves on port 8060, which is specified in `package.json` scripts section.
