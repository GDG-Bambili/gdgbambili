# GDG Bambili Website

[![forthebadge](https://forthebadge.com/images/badges/built-by-developers.svg)](https://github.com/gdg-bambili)
[![forthebadge](https://forthebadge.com/images/badges/contains-technical-debt.svg)](https://github.com/gdg-bambili)
[![forthebadge](https://forthebadge.com/images/badges/made-with-javascript.svg)](https://github.com/gdg-bambili)
[![forthebadge](https://forthebadge.com/images/badges/powered-by-black-magic.svg)](https://github.com/gdg-bambili)

- [Live demo](https://gdgbambili.dev)


## Features
* Material design
* Polymer
* Offline access
* Responsive
* Animations
* Integrated speakers and sessions management
* SVG icons
* SEO friendly
* Optimized and fast
* Editable theme colors
* ES2015 (compiles with Babel)
* Quick deploy


### Requirements
Project dependencies:

- Node.js used to run JavaScript tools from the command line.
- npm, the node package manager, installed with Node.js and used to install Node.js packages.
- gulp, a Node.js-based build tool.
- bower, a Node.js-based package manager used to install front-end packages (like Polymer).

**To install dependencies:**

1)  Check your Node.js version.

```sh
node --version
```

The version should be 0.12.x or above.

2)  If you don't have Node.js installed, or you have a lower version, go to [nodejs.org](https://nodejs.org) and click on the big green Install button.

3)  Install `gulp` and `bower` globally.

```sh
npm install -g gulp bower
```

This lets you run `gulp` and `bower` from the command line.

4)  Install the projects's local `npm` and `bower` dependencies.

```sh
cd gdg-bambili.xyz && npm install && bower install
```


### Modify to suit your needs
* Event info - [metadata folder](https://github.com/gdg-x/hoverboard/tree/master/app/metadata)
* Theme colors - [variables.css](https://github.com/gdg-x/hoverboard/tree/master/app/themes/hoverboard-theme/variables.css)
* Deployment [configs](https://github.com/gdg-x/hoverboard/tree/master/config.js)


### Development workflow
#### Initialize your app

```sh
gulp init
```

#### Serve / watch

```sh
gulp serve
```

This outputs an IP address you can use to locally test and another that can be used on devices connected to your network.

#### Build and serve the output from the dist build

```sh
gulp serve:dist
gulp serve:gae
```

#### Run tests

```sh
gulp test:local
```

#### Build & Vulcanize

```sh
gulp
```

### Deployment

GitHub Actions workflow on AWS S3

#### Deploy to development environment

```sh
gulp deploy:dev
```

#### Deploy to staging environment

```sh
gulp deploy:stag
```

#### Deploy to production environment

```sh
gulp deploy:prod
```

#### Promote the staging version to the production environment

```sh
gulp deploy:promote
```


### Tools

#### Download Google Fonts

Download Google Fonts for load page performance and offline using.
Fonts list for download is in file [fonts.list](https://github.com/gdg-x/hoverboard/blob/master/fonts.list).

```sh
gulp download:fonts
```

#### PageSpeed Insights

```sh
gulp pagespeed
```

#### Update versions of dependencies to the latest versions

```sh
# Install tool
npm install -g npm-check-updates

# Check latest versions
npm run check:ver # Alias for "ncu && ncu -m bower"

# Update to the latest versions
npm run update:ver # Alias for "ncu -u && ncu -um bower"
```


## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Make your changes
4. Run the tests, adding new ones for your own code if necessary
5. Commit your changes (`git commit -am 'Added some feature'`)
6. Push to the branch (`git push origin my-new-feature`)
7. Create new Pull Request


### Contributors

Maintainer: [@ch3ck](https://github.com/ch3ck).

## License

Project is published under the [MIT license](LICENSE.md)