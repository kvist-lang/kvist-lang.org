# kvist-lang.org

The website for [Kvist](https://github.com/kvist-lang/kvist), a practical Lisp
for native software that compiles to Odin.

The site is plain HTML and CSS and is published with GitHub Pages. The
documentation is generated as static HTML from the Markdown files in the main
Kvist repository.

To preview the homepage locally, run a static file server in this directory:

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Publishing

The Pages workflow builds and publishes the complete static site on every push
to `main`, when run manually, and every six hours so documentation changes in
[`kvist-lang/kvist`](https://github.com/kvist-lang/kvist) are picked up. The
custom domain is declared in `CNAME`; DNS is managed separately.

For a local documentation build, install the Node dependencies and pass the
path to a Kvist checkout:

```sh
npm install
npm run build:docs -- --source ../kvist/docs --output _site --config docs.config.json
```
