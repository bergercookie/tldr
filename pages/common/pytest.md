# pytest

> Testing framework for Python.

- Auto-discover and run all tests, including the doctests:

`pytest --doctest-modules`

- Auto-discover and run all tests, except those that match a regex:

`pytest --doctest-modules --ignore-glob={{some-regex}}`

- Do not capture standard output but dump it to the screen

`pytest -s`
