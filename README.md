[![Build Status][_self_:build-status:shield]][_self_:build-status] [![Dependencies Status][_self_:dependencies-status:shield]][_self_:dependencies-status] [![Node Version][_self_:node-version:shield]][_self_:node-version] [![License][_self_:license:shield]][BSD License] [![semantic-release][semantic-release:shield]][semantic-release] [![Commitizen friendly][commitizen:shield]][commitizen]

A personal [ESLint] config, but with ESLint itself and all the necessary shareable config, plugins, and parser as dependencies.

Provides a `lint` command which runs ESLint with this module's `.eslintrc` in the context of this module's dependencies, so I don't have to manage these dependencies in every project.

[![NPM][_self_:npm:badge]][_self_:npm]

## Table of Contents

<!-- MarkdownTOC autolink=true bracket=round -->

- [Installation](#installation)
- [Thanks](#thanks)
- [Troubleshooting](#troubleshooting)
- [Authors](#authors)
- [Contribute](#contribute)
- [License](#license)
- [Change Log](#change-log)

<!-- /MarkdownTOC -->

## Installation

Install this package:
```bash
$ npm install --save-dev eslint-config-sebastienbarre
```

then update your `package.json`:
```json
{
  "scripts": {
    "lint": "lint src tests"
  }
}
```

## Thanks

* [Jonny Buchanan][insin:github] for his [Config → Tools: ESLint][insin:eslint] post detailing this approach and implementing it in [insin/eslint-config-jonnybuchanan].

## Troubleshooting

For [roadhump/SublimeLinter-eslint] to keep linting, make sure to install this package globally and symlink `lint` to become the new `eslint`:
```bash
$ npm install -g eslint-config-sebastienbarre
$ cd ~/.npm-packages/bin
$ ln -s lint eslint
```

## Authors

**Sebastien Barre**

* Email: sebastien.barre@gmail.com
* Twitter: [sebastienbarre][sebastienbarre:Twitter]

## Contribute

* Check for [open issues][_self_:issues], especially the ones [up-for-grabs][_self_:issues:up-for-grabs], or open a fresh issue to start a discussion around a feature idea or a bug.
* If you feel uncomfortable or uncertain about an issue or your changes, feel free to [email me][sebastienbarre:email] and I will happily give you a hand.
* Fork the [repository][_self_:repo] on GitHub to start making your changes to the *master* branch (or branch off of it).
* Do *not* use `git commit` to commit your code; use `npm run commit` instead; this will ensure a [Commitizen]-friendly commit message will be generated, a convention that will in turn be leveraged by [semantic-release].
* Send a pull request and notify me :) Thanks.

## License

This software is released under the [BSD License].

## Change Log

All notable changes to this project are documented automatically on the Github [releases][_self_:releases] page. This project believes in [Semantic Versioning] and [Keep a CHANGELOG]. It uses [commitizen] and [semantic-release] to help with that endeavor.

[_self_:build-status:shield]: https://img.shields.io/travis/sebastienbarre/eslint-config-sebastienbarre.svg
[_self_:build-status]: https://travis-ci.org/sebastienbarre/eslint-config-sebastienbarre
[_self_:dependencies-status:shield]: https://img.shields.io/gemnasium/sebastienbarre/eslint-config-sebastienbarre.svg
[_self_:dependencies-status]: https://gemnasium.com/sebastienbarre/eslint-config-sebastienbarre
[_self_:issues:up-for-grabs]: https://github.com/sebastienbarre/eslint-config-sebastienbarre/labels/up-for-grabs
[_self_:issues]: https://github.com/sebastienbarre/eslint-config-sebastienbarre/issues
[_self_:license:shield]: https://img.shields.io/npm/l/eslint-config-sebastienbarre.svg
[_self_:node-version:shield]: https://img.shields.io/node/v/eslint-config-sebastienbarre.svg
[_self_:node-version]: https://www.npmjs.com/package/eslint-config-sebastienbarre
[_self_:npm:badge]: https://nodei.co/npm/eslint-config-sebastienbarre.png?downloads=true
[_self_:npm]: https://nodei.co/npm/eslint-config-sebastienbarre/
[_self_:releases]: https://github.com/sebastienbarre/eslint-config-sebastienbarre/releases
[_self_:repo]: https://github.com/sebastienbarre/eslint-config-sebastienbarre
[BSD License]: http://opensource.org/licenses/BSD-3-Clause
[commitizen:shield]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
[commitizen]: https://github.com/commitizen/cz-cli
[ESLint]: http://eslint.org/
[insin:github]: https://github.com/insin
[insin:eslint]: https://medium.com/@jbscript/config-tools-eslint-c85b6d48f7e2#.fvzzrrlfz
[insin/eslint-config-jonnybuchanan]: https://github.com/insin/eslint-config-jonnybuchanan
[Keep a CHANGELOG]: http://keepachangelog.com/
[roadhump/SublimeLinter-eslint]: https://github.com/roadhump/SublimeLinter-eslint
[sebastienbarre:email]: mailto:sebastien.barre@gmail.com
[sebastienbarre:Twitter]: https://twitter.com/sebastienbarre/
[Semantic Versioning]: http://semver.org/
[semantic-release:shield]: https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg
[semantic-release]: https://github.com/semantic-release/semantic-release
