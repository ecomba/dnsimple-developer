# DNSimple API Documentation

This is the DNSimple API documentation built with [nanoc](http://nanoc.ws/).

## Setup

Ruby 2 is required to build the site, all the dependencies are managed using Bundler, and yarn.

```shell
git clone https://github.com/dnsimple/dnsimple-developer.git
cd dnsimple-developer
bundle
yarn
```

For a list of `nanoc` commands type

```shell
nanoc --help
```

To build the openapi.json file, run `rake compile` before starting nanoc.

## Development

Use `yarn live` to concurrently compile JS and CSS dependencies along with running `nanoc live`.
An autocompiler automatically compiles changed files on every HTTP request.

```shell
yarn live

Loading site… done
11:56:37 - INFO - Compilation succeeded.
[2016-12-21 11:56:37] INFO  WEBrick 1.3.1
[2016-12-21 11:56:37] INFO  ruby 2.3.3 (2016-11-21) [x86_64-darwin16]
[2016-12-21 11:56:37] INFO  WEBrick::HTTPServer#start: pid=63695 port=3000
```

## Deployment

Each commit to master is deployed automatically via Netlify.
