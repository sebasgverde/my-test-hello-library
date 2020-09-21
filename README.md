# my-test-pypi-library
python library test and template for PyPI uploading

Links of tutorials for PyPI
- It has all the important instructions, used as main source: [https://packaging.python.org/tutorials/distributing-packages/](https://packaging.python.org/tutorials/distributing-packages/)
- More descriptive about the files and structure but still use only as complement and reference more in the first link [https://packaging.python.org/guides/migrating-to-pypi-org/#uploading](https://packaging.python.org/guides/migrating-to-pypi-org/#uploading)

After replace all the names in configuration files and folders and test that the folder works as a module using it in some code (this would be the internal folder with underscores, i.e my_test_hello_library, since the library folder won't be recognized as a module):

```
python setup.py sdist bdist_wheel
```

```
python -m twine upload --repository testpypi dist/*
```

Then, once you tested the libray in testpypi installing it in some virtual env and using it in python, the final step is upload it to the real pypi (for both cases remember have in hand you pypi and testpypi credentials)
```
python -m twine upload dist/*
```
