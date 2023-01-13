# Learn Sphinx

## References

[Official Sphinx Documentation](https://www.sphinx-doc.org/en/master/usage/quickstart.html)

[Document Your Scientific Project With Markdown, Sphinx, and Read the Docs | PyData Global 2021](https://www.youtube.com/watch?v=qRSb299awB0&t)

[Mariatta Wijaya - Introduction to Sphinx Docs and reStructuredText - Pyninsula #28](https://www.youtube.com/watch?v=v4eoYpCON_c)

https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/

https://kedro.readthedocs.io/en/stable/tutorial/package_a_project.html

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


## Notes 2 (for Kedro)

...



## Notes from official documentation

```
sphinx-build -b html sourcedir builddir
```
I try this from project root folder
```
sphinx-build -b html docs/source funny
```


## __The actual instructions I used__

Navigate to project root folder
```
# On anaconda powershell
cd C:\Users\Jansen-Lin\github-local-repo\learn-sphinx
```
Create `docs\` folder if haven't done so
```
mkdir docs
```

Create Virtual Environment
```
python -m venv .env
```

Activate the virtual environment
```
# On anaconda powershell
.env/Scripts/Activate.ps1

# On Git Bash
source .env/Scripts/activate

# On CMD
.env/Scripts/activate.bat
```

Install Sphinx in virtual environment
```
python -m pip install sphinx
```

Getting started on Sphinx
```
cd docs
sphinx-quickstart
```

Install choco
```
choco install make
```

To build the docs
```
cd docs

make html
```
The HTML pages created are found in `docs/build/html/`

Now you can open `docs/build/html/index.html` with your favourite browser.

Here is a third party extension to auto rebuild a documentation.
To install it...
```
python -m pip install sphinx-autobuild
```

To auto rebuild the docs...
Navigate to the project root
```
cd C:\Users\Jansen-Lin\github-local-repo\learn-sphinx
```
```
sphinx-autobuild docs docs/build/html
```

To deactivate 
```
deactivate
```
