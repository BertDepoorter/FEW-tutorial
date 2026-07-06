# FEW tutorial

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BertDepoorter/FEW-tutorial/blob/main/FEW_tutorial.ipynb)

Tutorial for GW workshop in Leuven 7th of July 2026

See [SETUP.md](SETUP.md) for local installation. To run in the browser with no
install, click the **Open in Colab** badge above and run this in the first cell:

```python
!pip install fastemriwaveforms
```

## Minimal_waveform_model (Robrecht Keijzer)

A minimal waveform model for adiabatic quasi-circular Schwarzschild orbits. All the main components for a full FEW model are present. Energy fluxes are from BHPT repo. Amplitudes are generated in a Mathematica notebook using the BHPT package.



---------------

## FEW  (Bert Depoorter)

Genereer zelfde waveform en toon visueel naast elkaar
- speedups: mode selection, snelle interpolatie met splines
- split in precomputed data - on the fly interpolatie via multi-dimensional splines -> very fast. 
- Verschillende waveform modellen geïmplementeerd:
	- Schwarzschild eccentric
	- KerrEEccentricEquatorial
	- frequency-domain waveform
	- 5PN-AAK kludge waveform -> do not use
- Outlook on the next waveform models, summarize Zach's slides op twee slides ofzo.
## Data analyse (30 min)

Toon waveform visuals: time domain, frequency domain, time-frequency domain
- Maak gif als in Ollie's repo.
- Update mode content plots
- Toon evolutie voor de waveform met mode selection threshold

Toon $\dot \Phi_{mn}$ op spectrogram and voeg gradueel meer modes toe. 

Compute mismatch voor perturbatie van parameters: kleine PE test

Toon evolutie likelihood voor parameters en toon impact van secondary modes. 



