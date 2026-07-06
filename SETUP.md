# Setup

The tutorial needs Python 3.12.12 and the [FastEMRIWaveforms](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms) package (`few`, v2.x). CPU-only is fine if you don't have a GPU, just slower. Only works with NVIDIA GPUs. 

## Option A: Google Colab (no install)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BertDepoorter/FEW-tutorial/blob/main/FEW_tutorial.ipynb)

Click the badge, then run the first cell to install dependencies:

```python
!pip install fastemriwaveforms
```

For a local install instead:

## Option B — conda 

```bash
conda create -n few2.0.0 python=3.12.12 -y
conda activate few2.0.0
pip install fastemriwaveforms
pip install -r requirements.txt
```

## Option C — uv

```bash
uv venv --python 3.12.12
source .venv/bin/activate          # Windows: .venv\Scripts\activate
uv pip install -r requirements.txt
```

## Option D — plain venv

```bash
python3.12 -m venv .venv
source .venv/bin/activate          # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Run the notebook

```bash
jupyter lab FEW_tutorial.ipynb
```

The first time you run a waveform, `few` downloads its data files automatically (needs an internet connection). This is about 5 GB of precomputed data, which only needs to be dowloaded once. There are many options to manage the data storage location, see the [few documentation](https://bhptoolkit.org/FastEMRIWaveforms/user/cfg.html#file-storage-path). The default location will work just fine for most users. 

## Check the install

```bash
python -c "import few; from few.waveform import FastKerrEccentricEquatorialFlux; print('FEW OK')"
```

## GPU (optional)

FEW runs on CPU out of the box. To use an NVIDIA GPU, additionally install the CuPy wheel matching your CUDA toolkit, e.g. `pip install cupy-cuda12x`.
