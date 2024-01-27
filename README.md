
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
wasmer run wasmer-examples/mkdocs-wasmer-starter --net -- --port 8000
```

> [!TIP]
> You can also run `wasmer run . --net -- --port 8000` in the root of this repo, after running `mkdocs build`


Open [http://localhost:8000](http://localhost:8000) with your browser to see the result.

## Deploy on Wasmer Edge

The easiest way to deploy your Mkdocs static site is to use the [Wasmer Edge](https://wasmer.io/products/edge).

Live example: https://wasmer-edge-mkdocs-sample.wasmer.app/

First, you'll need to run `mkdocs build`, and then, to deploy to Wasmer Edge:

```bash
wasmer deploy
```

> [!NOTE]
> You will need to have Wasmer installed (check out [the docs to install the Wasmer CLI](https://docs.wasmer.io/install)!). 
> You will also need to change the namespace in `wasmer.toml` to your own namespace and app name in `app.yaml` to your own app name.
