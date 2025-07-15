# CryoJAX-show-and-tell

Repository with examples for the Show and Tell session at the Computational Cryo-EM Workshop 2025 at Flatiron Institute.

## Requierements

Start by cloning this repo
```bash
git clone git@github.com:DSilva27/CryoJAX-show-and-tell.git
```

Prepare a python virtual environment. Make sure that the python version is 3.11 or higher, as this is required by cryojax:

```bash
python -m venv .venv
source .venv/bin/activate
```

you can check the python version by running `python --version`. If this is not >3.11, then you can try `python3.11 --version`. Hopefully `python3.11` will be defined in your path. If you are in a cluster you might need to load python 3.11 as a module by running something like `module load python/3.11`. Otherwise you will need to install python3.11 or create the environment using [conda](https://www.anaconda.com/docs/getting-started/miniconda/install)
```bash
conda create -n cryojax_tutorial_env python=3.11
conda activate cryojax_tutorial_env
```
or [uv](https://docs.astral.sh/uv/getting-started/installation/#standalone-installer)
```bash
uv venv --python 3.11
source .venv/bin/activate
```

Make sure your environment is activated and proceed to install the required libraries for the tutorial. If you are using `uv` replace `pip` with `uv pip`.

```bash
pip install cryojax
pip install jax-dataloader
pip install optax
```


