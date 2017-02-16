# Hugo Portfolio Website

This repo contains a working static website written with [Hugo](http://gohugo.io/), integrated with content coming from a [DatoCMS](https://www.datocms.com) administrative area.

## Usage

First, install the dependencies of this project:

```
yarn install
```

Then, to run this website in development mode (with live-reload):

```
yarn start
```

To build the final, production ready static website:

```
yarn build
```

The final result will be saved in the `public` directory.

## About

The goal of this project is to show how easily you can create static sites using the content (text, images, links, etc.) stored on [DatoCMS](https://www.datocms.com). This project is configured to fetch data from a specific administrative area using [the API DatoCMS provides](https://www.datocms.com/docs/api/sma/).

This websites uses:

* [Yarn](https://yarnpkg.com/) as package manager;
* [Webpack](https://webpack.github.io/) to compile and bundle assets (Sass/ES2015 JS);
* [datocms-client](https://github.com/datocms/js-datocms-client) to integrate the website with DatoCMS.

## The `dato.config.js` file

To convert the content stored on DatoCMS into local Markdown files that can be digested by Hugo, the datocms-client plugin requires an explicit mapping file called [`dato.config.js`](https://github.com/datocms/hugo-portfolio/blob/master/dato.config.js). You can read more about the commands available in this file [in the plugin documentation](https://github.com/datocms/js-datocms-client/blob/master/docs/dato-cli.md).


