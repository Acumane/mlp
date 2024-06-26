---
title: Home
layout: home
nav_order: 1
---

**MLP** is a fast inference server made in Python via Flask and a few other core Python libraries. Communication is handled via websockets.

## Installation 

Run the following commands to set up your environment.

```sh
git clone https://github.com/h3x4g0ns/mlp
cd mlp
conda create -n mlp_server python=3.11
conda activate mlp_server
pip install -r requirements.txt
```
## Getting Started

For running the server and client together run the following command:

```sh
python run.py

# basically runs the following commands under the hood
python mlp/src/server.py &
python examples/client.py
```

### Running unittests

For running unittests run the following command:

```sh
make test

# basically runs the following command under the hood
pytest
```
