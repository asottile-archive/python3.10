# DEPRECATED

Use the builds from https://github.com/deadsnakes/nightly instead

___

python3.10
==========

a repackage of cpython master on 2019-07-17 with the minor version bumped to
3.10

## tl;dr ppa

this is available as an [ubuntu PPA](https://launchpad.net/~asottile/+archive/ubuntu/python3.10)

```bash
sudo add-apt-repository ppa:asottile/python3.10
sudo apt-get update
sudo apt-get install python3.10-dev
```

## why do this?

there's a significant amount of code which uses `sys.version[:3]` which will
incorrectly report this as version `3.1` -- let's fix this long before it's a
problem!

## related projects

check out [flake8-2020](https://github.com/asottile/flake8-2020) for a flake8
plugin which checks for common related mistakes

## my suggestion

python3.10 breaks less code than python4.0

## some example fixes

- [pypa/virtualenv#1385](https://github.com/pypa/virtualenv/pull/1385)
- [tox-dev/tox#1377](https://github.com/tox-dev/tox/pull/1377)
- [pypa/setuptools#1824](https://github.com/pypa/setuptools/pull/1824)
