# entropy
## An example of directory structure for testing

To run tests, you must first install the entropy package with pip. Use:
`pip install --no-deps -e .`

(The option `--no-deps` tells pip not to install the dependencies, something we want to do because we manage our dependencies with conda, not pip. The option `-e` makes this an editable install so that if you change you don't have to reinstall to run the modified code.)

You can run the tests in the `tests` directory with:
`pytest`

A few things to note:
1. It is important to have an installable package, with an `__init__.py` file in the package directory and a `pyproject.toml`.
2. You must install the package to be able to run the tests.
3. Both the test files and the test functions must start with `test_` for pytest to find them.
4. In the `tests_entropy.py` file, do not use relative imports.