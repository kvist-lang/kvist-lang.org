# kvist-lang.org

The website for [Kvist](https://github.com/kvist-lang/kvist), a practical Lisp
for native software that compiles to Odin.

The site is plain HTML and CSS and is published with GitHub Pages. To preview it
locally, run a static file server in this directory, for example:

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Publishing

Changes pushed to `main` are published from the repository root. The custom
domain is declared in `CNAME`; DNS is managed separately.
