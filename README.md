
This is a [Mkdocs](https://www.mkdocs.org/) starter project that builds a static site based of Markdown files.

## Getting Started

First, install the dependencies:

```bash
pip install mkdocs
```

Then you can serve the mkdocs locally with:

```bash
mkdocs serve
```

Open [http://localhost:8000](http://localhost:8000) with your browser to see the result.

You can also build the static site directly with:

```bash
mkdocs build
```

Which will create the static-site inside the `site` directory.

## Deploy on Wasmer Edge

The easiest way to deploy your Mkdocs static site is to use the [Wasmer Edge](https://wasmer.io/products/edge).

Live example: http://wasmer-edge-mkdocs-sample.wasmer.app/

First, you'll need to run `mkdocs build`, and then, to deploy to Wasmer Edge:

```bash
wasmer deploy
```

> [!NOTE]
> You will need to have Wasmer installed (check out [the docs to install the Wasmer CLI](https://docs.wasmer.io/install)!). 
> You will also need to change the namespace in `wasmer.toml` to your own namespace and app name in `app.yaml` to your own app name.
