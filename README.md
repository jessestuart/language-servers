# language-servers

[![CircleCI](https://circleci.com/gh/palantir/language-servers.svg?style=svg)](https://circleci.com/gh/palantir/language-servers)
[![Download](https://api.bintray.com/packages/palantir/releases/language-servers/images/download.svg)](https://bintray.com/palantir/releases/language-servers/_latestVersion)

A collection of implementations for the
[Microsoft Language Server Protocol](https://github.com/Microsoft/language-server-protocol/blob/master/protocol.md)

## Included projects

### groovy-language-server

A groovy implementation of the protocol. Uses the Java API definition in
[typefox/ls-api](https://github.com/TypeFox/ls-api)

### language-server-commons

A framework that makes writing additional light-weight language-servers easier.

## Dev Setup

### Getting started

This project requires a working installation of JDK 8.

```shell
$ git clone https://github.com/palantir/language-servers
$ cd language-servers
# Optional: generate IDE project files for Eclipse or IntelliJ.
$ ./gradlew eclipse # OR `./gradlew idea`
```

### Building and Testing

```shell
# Compiles, runs tests, checkstyle and findbugs.
$ ./gradlew build
# Runs all unit tests.
$ ./gradlew test
# Creates jars in your Maven local repository.
$ ./gradlew publshToMavenLocal
```

### Debug

```shell
# Deletes gradle generated files.
$ ./gradlew clean cleanEclipse cleanIdea
```
