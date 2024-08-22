
This is a [Mkdocs](https://www.mkdocs.org/) starter project that builds a static site based of Markdown files.

## Getting Started

First, install the dependencies:

```bash
pip install mkdocs
```

You can also build the static site directly with:

```bash
mkdocs build
```

Which will create the static-site inside the `site` directory.

Then you can serve the mkdocs locally with:

```bash
mkdocs serve
```

You can also run the Mkdocs project easily using Wasmer (check out the [install guide](https://docs.wasmer.io/install)):

```bash
mkdocs build
wasmer run . -- --port 8000
```

Open [http://localhost:8000](http://localhost:8000) with your browser to see the result.

## Deploy on Wasmer Edge

The easiest way to deploy your Mkdocs static site is to use the [Wasmer Edge](https://wasmer.io/products/edge).

Live example: https://wasmer-edge-mkdocs-sample.wasmer.app/

First, you'll need to run `mkdocs build`, and then, to deploy to Wasmer Edge:

```bash
wasmer deploy
```
