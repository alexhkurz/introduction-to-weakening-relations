# README

## Jupyter Books

This book has been created with jupyter books following [these steps(https://alexhkurz.github.io/introduction-to-jupyter-book). To build the book and open it locally in your web browser run (if you are on a mac)

```
jb build . ; open _build/html/index.html
```

```
git init
git branch -m main
git add *
git commit -m "initial commit"
```

To create a repo in the cloud go to a git server such as [Github](https://github.com/). 

Create an empty public repository at Github. Then run locally:

```
git remote add origin https://github.com/alexhkurz/introduction-to-jupyter-book.git
git push -u origin main
```

Since then the files are available at [`https://github.com/alexhkurz/introduction-to-jupyter-book`](https://github.com/alexhkurz/introduction-to-jupyter-book).


### Publishing

Following [Publish your book online](https://jupyterbook.org/en/stable/start/publish.html) install `ghp-import`

```
pip install ghp-import
```

and then publish the book by running

```
ghp-import -n -p -f _build/html
```

This makes the book available online at 

[`https://alexhkurz.github.io/introduction-to-jupyter-book`](https://alexhkurz.github.io/introduction-to-jupyter-book) 

(possibly after some waiting time). It also keeps the source files in the `main`-branch separate from the files in `_build` in the `gh-pages` branch.

### important commands

If, for example, the table of contents in the left-hand pane behaves in a strange way, clean out `_build`:

```
jupyter-book clean .
```
