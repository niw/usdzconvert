usdzconvert
===========

A patched version of `usdzconvert` introduced in [Working with USD](https://developer.apple.com/videos/play/wwdc2019/602/?time=390)
presentation at WWDC19.
It can be used to convert from GLB to USDZ with recent Python 3.10
and `usd-core` module, which available on recent macOS and other platforms.

> NOTE: The script only patched for converting from GLB to USDZ,
> may not work with other use cases and may require similar changes in different code path.

Usage
-----

Install Python 3.10 by using, for example, Homebrew.
Use virtualenv and install dependencies, then use `usdzconvert`.
You can ignore error from `usdARKitChecker`.

```
$ brew install python@3.10
$ python3.10 -m venv .venv
$ .venv/bin/pip3 install -r requirements.txt
$ .venv/bin/python3 usdzconvert path-to-glb path-to-usdz
```
