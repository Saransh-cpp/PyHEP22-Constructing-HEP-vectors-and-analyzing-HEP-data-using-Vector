# PyHEP 2022 Notebook talk - Constructing HEP vectors and analyzing HEP data using Vector

[![Talk](https://img.shields.io/badge/PyHEP22-notebook_talk-blue?logo=github&logoColor=white&color=blue)](https://indico.cern.ch/event/1150631/contributions/5014393/)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Saransh-cpp/PyHEP22-Constructing-HEP-vectors-and-analyzing-HEP-data-using-Vector/HEAD?urlpath=lab/tree/talk.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Saransh-cpp/PyHEP22-Constructing-HEP-vectors-and-analyzing-HEP-data-using-Vector/blob/main/talk.ipynb)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7081003.svg)](https://doi.org/10.5281/zenodo.7081003)

[Vector](https://iris-hep.org/projects/vector.html) is a Python library for 2D, 3D, and Lorentz vectors, including arrays of vectors, designed to solve common physics problems in a NumPy-like way. Vector currently supports pure Python Object, NumPy, Awkward, and Numba-based (Numba-Object, Numba-Awkward) backends.

This talk will focus on introducing Vector and its backends to the HEP community through a data analysis pipeline. The session will build up from pure Python Object based vectors to Awkward based vectors, ending with a demonstration of Numba support. Furthermore, we will discuss the latest developments in the library's API and showcase some recent enhancements.

## Setup

There are two ways to follow along (or run this notebook after the talk) -

1. Locally

    - Clone [this](https://github.com/Saransh-cpp/PyHEP22-Constructing-HEP-vectors-and-analyzing-HEP-data-using-Vector.git) repository -
    ```bash
    git clone https://github.com/Saransh-cpp/PyHEP22-Constructing-HEP-vectors-and-analyzing-HEP-data-using-Vector.git
    ```

    - Change directory
    ```bash
    cd Constructing-HEP-vectors-and-analyzing-HEP-data-using-Vector
    ```

    - Launch the classic Jupyter notebook or Jupyter lab -
    ```bash
    jupyter notebook
    # or
    jupyter lab
    ```

2. On cloud (recommended)

    - Binder (recommended)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Saransh-cpp/PyHEP22-Constructing-HEP-vectors-and-analyzing-HEP-data-using-Vector/HEAD?urlpath=lab/tree/talk.ipynb)

    - Google Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Saransh-cpp/PyHEP22-Constructing-HEP-vectors-and-analyzing-HEP-data-using-Vector/blob/main/talk.ipynb)

We will be directly importing `vector`, `awkward`, `numpy`, `numba`, `uproot`, `matplotlibn`, and `scikit-hep-testdata` in this tutorial. Hence, a user must install these packages if this notebook is being run locally or on Google Colab.

## Recent developments

Vector [`v0.9.0`](https://github.com/scikit-hep/vector/releases/tag/v0.9.0) is out!
- Features: improved reprs, deltaRapidityPhi, backends are public now, …
- Documentation: major documentation overhaul, doctests, CITATION.cff, …
- Bug fixes: type checks, fix nan_to_num, …
- Maintenance: hatchling backend, support awkward._v2 in tests, build and test on Python 3.10 and 3.11-dev, …

More about `v0.9.0` here - https://vector.readthedocs.io/en/latest/changelog.html#version-0-9

---

Vector [`v0.10.0`](https://github.com/scikit-hep/vector/releases/tag/v0.10.0) is out too!
- Removed support for Python 3.6

More about `v0.10.0` here - https://vector.readthedocs.io/en/latest/changelog.html#version-0-10

## Near future development plans

- Better constructors (under work)
- A benchmarking suite
- Benchmarks against Root
- A complete `awkward` `v2` support (scheduled for December)
- NumPy-Numba backend
- Other potential backends -

Vector was scheduled to have a major release (`v1.0.0`) before `PyHEP 2022`, but that was unfortunately delayed. A major release can be expected in October, which would primarily be introducing new constructors.

Open for user feedback and discussions!

## Stuck somewhere? Reach out!

- If something is not working the way it should, or if you want to request a new feature, create a [new issue](https://github.com/scikit-hep/vector/issues) on GitHub.
- To discuss something related to vector, use the [discussions](https://github.com/scikit-hep/vector/discussions/) tab on GitHub or vector’s gitter ([Scikit-HEP/vector](https://gitter.im/Scikit-HEP/vector)) chat room.
- Have a look at vector's [changelog](https://vector.readthedocs.io/en/latest/#changes-in-vector-s-api) to stay up-to-date!

## Cite vector

If you use `vector` in your work, please cite it using the following metadata -

```bib
@software{Schreiner_vector,
author = {Schreiner, Henry and Pivarski, Jim and Chopra, Saransh},
doi = {10.5281/zenodo.5942082},
license = {BSD-3-Clause},
title = {{vector}},
url = {https://github.com/scikit-hep/vector}
}
```
