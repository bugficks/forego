![latest 0.21.0](https://img.shields.io/badge/latest-0.21.0-green.svg?style=flat)
[![CircleCI](https://circleci.com/gh/bugficks/forego.svg?style=svg)](https://circleci.com/gh/bugficks/forego)
![Apache 2.0](https://img.shields.io/badge/license-Apache%202-blue.svg?style=flat)
![Go Version](https://img.shields.io/github/go-mod/go-version/bugficks/forego)

## forego
[Foreman](https://github.com/ddollar/foreman) in Go.

Changes:
+ [Fix accidentally stateful port calculation #105](https://github.com/ddollar/forego/pull/105)
+ [Add NO_COLOR, inject version tag, and more #124](https://github.com/ddollar/forego/pull/124)
+ [Add procNum to the port calculation for startProc #1](https://github.com/bugficks/forego/pull/1)

### Installation

[Downloads](https://github.com/bugficks/forego/releases)

##### Compile from Source

    $ go get -u github.com/bugficks/forego

### Usage

    $ cat Procfile
    web: bin/web start -p $PORT
    worker: bin/worker queue=FOO

    $ forego start
    web    | listening on port 5000
    worker | listening to queue FOO

Use `forego help` to get a list of available commands, and `forego help
<command>` for more detailed help on a specific command.

### License

Apache 2.0 &copy; 2015 David Dollar
