# Twine

> Twine is a utility for publishing Python packages on PyPI.

- Install prerequisites:

`pip3 install --user --upgrade setuptools wheel twine`

- Build a package:

`python3 setup.py sdist bdist_wheel`

- Upload a package to test.pypi:

`twine upload --repository-url https://test.pypi.org/legacy/ dist/*`

- Deploy a package:

`twine upload dist/*`

- Remember to bump the setup.py version:

`HTTPError: 400 Client Error: File already exists`

- Update your twine version - you may be way behind:

`HTTPError: 400 Client Error: The description failed to render in the default format of reStructuredText.`
