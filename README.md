### `blis` and `spacy` wheels for `cp37-cp37m-linux_armv7l`

`blis==0.4.1` and `spacy==2.2.3` wheels for `cp37-cp37m-linux_armv7l` arch, built on a RPi 3 (`cortex a15`), Raspbian Buster.

Build steps can be found in [this answer on SO](https://stackoverflow.com/a/59957172/2650249).

### Installing using PyPI index proxy

```sh
$ pip install spacy --extra-index-url=https://hoefling.io/pypi
```
`https://hoefling.io/pypi` simply proxies `pip install` requests to GitHub release page.

### Installing from Github releases

```sh
$ pip install https://github.com/hoefling/so-59927844/releases/download/0.1/blis-0.4.1-cp37-cp37m-linux_armv7l.whl
$ pip install https://github.com/hoefling/so-59927844/releases/download/0.1/spacy-2.2.3-cp37-cp37m-linux_armv7l.whl
```
