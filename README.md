# zinit-annex-test

## Introduction

A [zinit](https://github.com/zdharma-continuum/zinit) extension (i.e. an
[annex](https://zdharma-continuum.github.io/zinit/wiki/Annexes/)) that runs tests (via `make
test`, for example) – if it finds any of them  – after installing and updating
a plugin or snippet. Simply load it like any other plugin to make it active:

```zsh
zinit light zdharma/z-p-test
```

## Configuration

To run the tests in a verbose mode, issue:

```zsh
zstyle :zinit:annex:test quiet 0
```

before installing or updating the plugin. To skip tests for a single plugin,
add `notest` ice:

```zsh
zinit ice notest
zinit load …
```

## Examples

Example activation in the default quiet mode:

![z-p-test activation](https://raw.githubusercontent.com/zdharma-continuum/zinit-annex-test/master/images/z-p-test-1.png)


Example activation in non-quiet mode:

![z-p-test activation](https://raw.githubusercontent.com/zdharma-continuum/zinit-annex-test/master/images/z-p-test-2.png)

<!-- vim:set ft=markdown:tw=80: -->
