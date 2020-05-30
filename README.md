### `blis` and `spacy` wheels for `cp37-cp37m-linux_armv7l` and `cp37-cp37m-linux_aarch64`

`blis==0.4.1` and `spacy==2.2.3` wheels for `cp37-cp37m-linux_armv7l` and `cp37-cp37m-linux_aarch64` arches. `armv7l` wheels  built on a RPi 3 (target CPU: Cortex-A15), Raspbian Buster; `aarch64` wheels built on RPi 4 in the `manylinux2014` container (target CPU: Cortex-A57).

Build steps can be found in [this answer on SO](https://stackoverflow.com/a/59957172/2650249).

### Installing using PyPI index proxy

```sh
$ pip install spacy --extra-index-url=https://hoefling.io/pypi
```
`https://hoefling.io/pypi` simply proxies `pip install` requests to GitHub release page.

### Installing from Github releases

`armv7l`:

```sh
$ pip install https://github.com/hoefling/so-59927844/releases/download/0.1/blis-0.4.1-cp37-cp37m-linux_armv7l.whl
$ pip install https://github.com/hoefling/so-59927844/releases/download/0.1/spacy-2.2.3-cp37-cp37m-linux_armv7l.whl
```

`aarch64`:

```sh
$ pip install https://github.com/hoefling/so-59927844/releases/download/0.2/blis-0.4.1-cp37-cp37m-manylinux2014_aarch64.whl
$ pip install https://github.com/hoefling/so-59927844/releases/download/0.2/spacy-2.2.4-cp37-cp37m-manylinux2014_aarch64.whl
```
