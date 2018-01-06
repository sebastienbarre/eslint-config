<img src="https://gist.githubusercontent.com/sebastienbarre/6f8ce4bc7488bbd2238801eaa8a58fc9/raw/42414fef149734b8e757f986de1327c76432c941/separator.png" />

# ESLint Config

[![Build Status][_self_:build-status:badge]][_self_:build-status] [![License][BSD License:badge]][BSD License] [![NPM][_self_:npm:badge]][_self_:npm] [![semantic-release][semantic-release:badge]][semantic-release] [![Commitizen friendly][commitizen:badge]][commitizen]

A personal [ESLint] config, but with ESLint itself and all the necessary shareable config, plugins, and parser as dependencies.

Provides an `eslint` command which runs ESLint with this module's `.eslintrc` in the context of this module's dependencies, so I don't have to manage these dependencies in every project.

## Table of Contents

<!-- MarkdownTOC autolink=true bracket=round -->

- [Installation](#installation)
- [Thanks](#thanks)
- [Troubleshooting](#troubleshooting)
- [Authors](#authors)
- [Contribute](#contribute)
- [License](#license)
- [Changelog](#changelog)

<!-- /MarkdownTOC -->

## Installation

Install this package:
```bash
$ yarn add --dev @sebastienbarre/eslint-config
```

then update your `package.json`:
```json
{
  "scripts": {
    "lint": "eslint src tests"
  }
}
```

## Thanks

* [Jonny Buchanan][insin:github] for his [Config → Tools: ESLint][insin:eslint] post detailing this approach and implementing it in [insin/eslint-config-jonnybuchanan].

## Troubleshooting

For [roadhump/SublimeLinter-eslint] to lint with these settings, make sure to install this package globally:
```bash
$ yarn global add @sebastienbarre/eslint-config
```

## Authors

**Sebastien Barre**

* Email: sebastien.barre@gmail.com
* Web: http://barre.io
* Twitter: [sebastienbarre][sebastienbarre:Twitter]

## Contribute

* Check for [open issues][_self_:issues], especially the ones already [available][_self_:issues:available], or open a fresh issue to start a discussion around a feature idea or a bug.
* If you feel uncomfortable or uncertain about an issue or your changes, feel free to [email me][sebastienbarre:email] and I will give you a hand.
* Fork the [repository][_self_:repo] on GitHub to start making your changes to the *master* branch (or branch off of it).
* Write a test which shows that a bug exists, was fixed, or that a feature works as expected.
* Use `npm run commit` instead of `git commit` if you are unfamiliar with the [conventional-changelog] guidelines; this will ensure a [Commitizen]-friendly commit message will be generated, a convention that will in turn be leveraged by [semantic-release].
* Send a pull request and notify me :) Thanks.

## License

This software is released under the [BSD License].

## Changelog

All notable changes to this project are documented automatically on the Github [releases][_self_:releases] page. This project believes in [Semantic Versioning] and [Keep a CHANGELOG]. It uses [commitizen] and [semantic-release] to help.

[_self_:build-status:badge]: https://img.shields.io/travis/sebastienbarre/eslint-config.svg
[_self_:build-status]: https://travis-ci.org/sebastienbarre/eslint-config
[_self_:issues:available]: https://github.com/sebastienbarre/eslint-config/labels/Status%3A%20Available
[_self_:issues]: https://github.com/sebastienbarre/eslint-config/issues
[_self_:npm:badge]: https://img.shields.io/npm/v/@sebastienbarre/eslint-config.svg
[_self_:npm]: https://www.npmjs.com/package/@sebastienbarre/eslint-config
[_self_:releases]: https://github.com/sebastienbarre/eslint-config/releases
[_self_:repo]: https://github.com/sebastienbarre/eslint-config
[BSD License:badge]: https://img.shields.io/badge/license-BSD--3--Clause-blue.svg
[BSD License]: http://opensource.org/licenses/BSD-3-Clause
[commitizen:badge]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
[commitizen]: https://github.com/commitizen/cz-cli
[ESLint]: http://eslint.org/
[insin/eslint-config-jonnybuchanan]: https://github.com/insin/eslint-config-jonnybuchanan
[insin:eslint]: https://medium.com/@jbscript/config-tools-eslint-c85b6d48f7e2#.fvzzrrlfz
[insin:github]: https://github.com/insin
[Keep a CHANGELOG]: http://keepachangelog.com/
[roadhump/SublimeLinter-eslint]: https://github.com/roadhump/SublimeLinter-eslint
[sebastienbarre:email]: mailto:sebastien.barre@gmail.com
[sebastienbarre:Twitter]: https://twitter.com/sebastienbarre/
[Semantic Versioning]: http://semver.org/
[semantic-release:badge]: https://img.shields.io/badge/%F0%9F%93%A6-semantic--release-e10079.svg
[semantic-release]: https://github.com/semantic-release/semantic-release
