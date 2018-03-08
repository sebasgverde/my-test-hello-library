# my-test-hello-library
python library test and template for PyPI uploading

linsk of tutorials for PyPI
- [https://packaging.python.org/tutorials/distributing-packages/](https://packaging.python.org/tutorials/distributing-packages/)
- [https://gist.github.com/gboeing/dcfaf5e13fad16fc500717a3a324ec17](https://gist.github.com/gboeing/dcfaf5e13fad16fc500717a3a324ec17)
- [https://packaging.python.org/guides/migrating-to-pypi-org/#uploading](https://packaging.python.org/guides/migrating-to-pypi-org/#uploading)
- [http://python-packaging.readthedocs.io/en/latest/minimal.html](http://python-packaging.readthedocs.io/en/latest/minimal.html)

After replace all the names and test that the folder works as a module using it in some code:

```
python setup.py sdist bdist_wheel
```

```
twine upload dist/*
```