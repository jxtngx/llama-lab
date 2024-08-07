# LM Lab

## Overview

LM Lab is a template for language model pretraining, finetuning, and applied agents. 

## Project Structure

<details>
    <summary>root</summary>

`checkpoints` directory contains training checkpoints and the pre-trained production model.

`data` directory for local data caches.

`docs` directory for technical documentation.

`logs` directory contains logs generated from experiment managers and profilers.

`notebooks` directory can be used to present EDA and demo notebooks.

`requirements` directory of requirement files titled by purpose.

`tests` module contains unit and integration tests targeted by pytest.

`setup.py` `setup.cfg` `pyproject.toml` and `MANIFEST.ini` assist with packaging the Python project.

`.pre-commit-config.yaml` is required by pre-commit to install its git-hooks.

</details>

<details>
    <summary>src</summary>

`lmlab.data/` contains the CLI application implemented with Typer.

`lmlab.data/` contains code for preprocessing pipelines and PyTorch dataset utilities.

`lmlab.models/` contains code for model architectures implemented in PyTorch.

`lmlab.observe/` contains code for model observability.

`lmlab.serve/` contains code to serve a selected model.

`lmlab.train/` contains code for several varieties of Trainers.

`lmlab.tune/` contains code for HPO runs and sweeps.

`lmlab.utils/` contains utility functions.

</details>


## Installation

The recommended installation is as follows:

```sh
python3 -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
```
