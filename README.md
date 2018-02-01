# speccy

![Build](https://img.shields.io/travis/wework/speccy/master.svg)
[![Coverage Status](https://coveralls.io/repos/github/wework/speccy/badge.svg?branch=master)](https://coveralls.io/github/wework/speccy?branch=master)
[![Known Vulnerabilities](https://snyk.io/test/npm/speccy/badge.svg)](https://snyk.io/test/npm/speccy)

Enforce quality rules on your OpenApi 3.0.x specifications.

Currently tracking [v3.0.0](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.0.md)

```
Usage: speccy <command> [options] <file-or-url>


Options:

  -V, --version  output the version number
  -h, --help     output usage information


Commands:

  lint [options] <file-or-url>  Ensure your OpenAPI files are valid and up to scratch
```

## Features

### Rules

By default the [base](/rules/base.json) rules are used, but you can create your own rules files to use.

Contributions of rules and rule actions for the linter are very much appreciated.

## Tests

To run the test-suite:

```shell
yarn test
```

## Contributions

This package is forked from [swagger2openapi], written by [Mike Ralphson]. He'd written some linter functionality into that package's validator, and we outright lifted that straight from his code. This codebase will diverge and focus on building more, and more powerful rules, whilst that project is going to focus on OpenAPI v2 -> v3 conversion.

## License

[BSD-3-Clause](LICENSE) except the `openapi-3.0.json` schema, which is taken from the [OpenAPI-Specification](https://github.com/OAI/OpenAPI-Specification/blob/49e784d7b7800da8732103aa3ac56bc7ccde5cfb/schemas/v3.0/schema.yaml) and the alternative `gnostic-3.0.json` schema, which is originally from [Google Gnostic](https://github.com/googleapis/gnostic/blob/master/OpenAPIv3/openapi-3.0.json). Both of these are licensed under the [Apache-2](http://www.apache.org/licenses/LICENSE-2.0) license.

[swagger2openapi]: https://github.com/Mermade/swagger2openapi/
[Mike Ralphson]: https://twitter.com/PermittedSoc/
