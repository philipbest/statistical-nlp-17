# Statistical NLP (Group 17)

This is the repository for Group 17 of the Statistical Natural Language
Processing module at UCL, formed by:

- Talip Ucar
- Adrian Swarzc
- Matt Lee
- Adrian Gonzalez-Martin

## Getting Started

To keep the environments as reproducible as possible, we will use `pipenv` to
handle dependencies. Feel free to use `conda` or other tools which manage global
deps as well!

To install `pipenv` just follow the instructions in https://pipenv.readthedocs.io/en/latest/.

The first time, to create the environment and install all required dependencies,
just run

```console
$ pipenv install
```

This will create a `virtualenv` and will install all required dependencies.

### Installing new dependencies

To add new dependencies just run

```console
$ pipenv install numpy
```

Remember to commit the updated `Pipfile` and `Pipfile.lock` files so that
everyone else can also install them!

## Source Code

This repo should be treated as the single source of truth for source code,
therefore we should keep most of it as a library under the `src/` folder, so
that notebooks (or `ipython`, Colab, etc.) can just do something like

```python
from .src.models import MatchingNetworks
```

This way we avoid fragmentation across notebooks. This is also the most
platform-agnostic method as it's more generic and doesn't make any assumptions
on where the code will be run.
