# README

## Jupyter Books

This book can be viewed [here](https://alexhkurz.github.io/introduction-to-weakening-relations) has been created with jupyter books following [these steps](https://alexhkurz.github.io/introduction-to-jupyter-book). To build the book and open it locally in your web browser run (if you are on a mac)

```
jb build . ; open _build/html/index.html
```

To publish a new version run

```
ghp-import -n -p -f _build/html
```

If, for example, the table of contents in the left-hand pane behaves in a strange way, clean out `_build`:

```
jb clean .
```
