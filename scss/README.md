# Sass for this theme `Blue`

## Compile scss files

We need node module, `node-sass`, `nodemon` to auto compile scss files.

``` sh
npm install node-sass nodemon -g
```

Then using the command below to build css files:

``` sh
npm run build-css
```

You can also using the command below to auto-compile scss files when files changed.

``` sh
npm start
```

## Scss files and css files

The command above will compile this two files:

```
bootstrap-docs/bootstrap-docs.scss => /static/css/bootstrap-docs.min.css
material/materialize.scss => /static/css/material.min.css
```

And their sourcemap files will be storaged in:

```
bootstrap-docs/bootstrap-docs.scss => /static/css/bootstrap-docs.min.css.map
material/materialize.scss => /static/css/material.min.css.map
```
