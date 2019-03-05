# Saturation Playground (fork of [Deep Playground](https://github.com/tensorflow/playground))

![saturation_demo.gif](saturation_demo.gif)

About **saturation**: 

- a metric implemented in [Delve](https://github.com/justinshenk/delve) for identifying the diversity of inputs to a layer.
- layer saturation appears above the layer. High saturation (yellow or red) indicates increasing the layer size.

## Development

To run the visualization locally, run:
- `npm i` to install dependencies
- `npm run build` to compile the app and place it in the `dist/` directory
- `npm run serve` to serve from the `dist/` directory and open a page on your browser.

For a fast edit-refresh cycle when developing run `npm run serve-watch`.
This will start an http server and automatically re-compile the TypeScript,
HTML and CSS files whenever they change.

## For owners
To push to production: `git subtree push --prefix dist origin gh-pages`.

This is not an official Google product.
