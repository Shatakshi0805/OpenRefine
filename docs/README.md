How to build these docs
=======================

We use [Docusaurus 2](https://v2.docusaurus.io/) for our docs, a modern static website generator.

### Requirements
Assuming you have [Node.js](https://nodejs.org/en/download/) installed (which includes npm), you can install Docusaurus with:

You will need to install [Yarn](https://yarnpkg.com/getting-started/install) before you can build the site.
```sh
npm install -g yarn
```

### Installation

Once you have installed yarn, navigate to docs directory & set-up the dependencies.

```sh
cd docs
yarn
```

### Local Development

```sh
yarn start
```

This command starts a local development server and opens up a browser window. Usually at the URL http://localhost:3000
Most changes are reflected live without having to restart the server.

### Next version of OpenRefine docs
If you wish to work on the next version of docs for OpenRefine (`master` branch) then you will need to:
1. Git checkout our `master` branch
2. Edit files under `docs/docs/`
3. Preview changes with the URL kept pointing to http://localhost:3000/next which will automatically show changes live with yarn after you save a file.

### Build

```sh
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

```sh
GIT_USER=<Your GitHub username> USE_SSH=true yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
