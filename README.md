# Learn Sphinx

## References

[Official Sphinx Documentation](https://www.sphinx-doc.org/en/master/usage/quickstart.html)

[Document Your Scientific Project With Markdown, Sphinx, and Read the Docs | PyData Global 2021](https://www.youtube.com/watch?v=qRSb299awB0&t)

[Mariatta Wijaya - Introduction to Sphinx Docs and reStructuredText - Pyninsula #28](https://www.youtube.com/watch?v=v4eoYpCON_c)

https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/

## Notes

__reStructuredText__ <br>
(*rst)
- Is a markup language (like Markdown and HTML)
- Not as lightweight as Markdown
- Virtually unknown outside Python Community
- Used in Python since 2002
- PEP 287
- Python Docs & PEPs are written in it

__Markdown__
- Did not exist until 2004

__Sphinx__
- is a Documentation Generator
- Converts .rst into .html files <br>
  ...and other formats like PDF, EPub, etc

Why is python using .rst?
- ...

Get Started with Sphinx

```
python3 -m venv .env
source .env/bin/activate
python -m pip install sphinx
```
```
mkdir docs
cd docs
sphinx-quickstart
```

Finished: An initial directory structure has been created.

```yaml
/docs/
/docs/_build/
/docs/_static/
/docs/_templates/
/docs/conf.py
/docs/index.rst
/docs/make.bat
/docs/Makefile
```

__Build the Docs__

```
make html
```

The HTML pages are in _build/html.

`/docs/_build/html/index.html`

__sphinx-autobuild__

You can install a third party extension...
```
python3 -m pip install sphinx-autobuild
```

sphinx-autobuild docs docs/_build/html










