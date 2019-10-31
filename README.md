# Saturation Playground (fork of [Deep Playground](https://github.com/tensorflow/playground))

![saturation_demo.gif](saturation_demo.gif)

About **saturation**: 

- a metric implemented in [Delve](https://github.com/justinshenk/delve) for identifying the diversity of inputs to a layer.
- two options for calculating saturation (via principal components of neuron preactivation-states over training): "Simpson diversity index" and "Cumulative 99"
- layer saturation appears above the layer. High saturation (yellow or red) indicates increasing the layer size.

Read about it in "Spectral Analysis of Latent Representations" [arXiv](https://arxiv.org/abs/1907.08589) and please cite as:

```
@misc{shenk2019spectral,
    title={Spectral Analysis of Latent Representations},
    author={Justin Shenk and Mats L. Richter and Anders Arpteg and Mikael Huss},
    year={2019},
    eprint={1907.08589},
    archivePrefix={arXiv},
    primaryClass={cs.LG}
}
```

Instructions from the source repo:

## Development

To run the visualization locally, run:
- `npm i` to install dependencies
- `npm run build` to compile the app and place it in the `dist/` directory
- `npm run serve` to serve from the `dist/` directory and open a page on your browser.

For a fast edit-refresh cycle when developing run `npm run serve-watch`.
This will start an http server and automatically re-compile the TypeScript,
HTML and CSS files whenever they change.
