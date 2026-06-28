
Presentatie - tutorial met FEW


TODO: git repo maken voor de notebooks en environment
## Inleiding (30 min)

Introductie EMRI waveforms: orbits, two-timescale expansion, 
post-adiabatic waveforms -> toon effect op PE en bias
State of the art: aligned spin, slowly spinning primary, evolution chi1 and m1 included

Waveform constructie:
[EQ here]

Two-timescale analysis: amplitudes evolueren traag, phases moeten heel nauwkeurig geïntegreerd worden. 

Twee delen: harmonic mode decomposition and exploit GPU 

fase: ODEs van forced geodesics

[toon in code Robrecht]

amplitudes: amplitude, spin-weighted spherical harmonics, polarizatie

[toon in code Robrecht]

Teukolsky eq. met bron 

Flowchart maken hoe code doorlopen wordt. 

Waveform constructie: verschillende delen samenbrengen, roteren naar detector-frame -> finale waveform

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



