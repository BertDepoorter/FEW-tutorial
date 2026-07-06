

TODO: git repo maken voor de notebooks en environment
## Minimal_waveform_model

A minimal waveform model for adiabatic quasi-circular Schwarzschild orbits. All the main components for a full FEW model are present.



---------------

## FEW  (10 min install + 20 min walkthrough)

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



