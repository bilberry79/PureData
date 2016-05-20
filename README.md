# PureData
PureDate patches and abstracts

<h3>Audio analyzer</h3>
`[abs_spec_duo]` : A tool to visualize the frequency spectrum and the wave form of two audio inputs. 
![alt text](https://github.com/bilberry79/PureData/blob/master/pictures/abs_spec_duo.PNG)

`[abs_spec]` : A tool to visualize the frequency spectrum in a <b>logarithmic</b> and linear view of one audio input.

`[abs_spec_comp]` : A compact version of [abs_spec_duo] with only one input.
![alt text](https://github.com/bilberry79/PureData/blob/master/pictures/abs_spec_comp.PNG)

<h3>Dynamic Block Switching Synthesis</h3>
`DBS.pd`

This tool proposes a new sound synthesis algorithm based on dynamic block switching techniques used in common MP3 compression. After the transformation of the analysis signal in the frequency domain (STFT), a transient detection algorithm triggers the block switching decisions that synthesize a new sound. Block sizes of 128-8192 samples are possible. Smaller block sizes assure a more precise localisation of the audio event in time and larger block sizes smear the onset of an event in time but provide a richer overtone spectrum. Several spectral effects are available to give the user a broad toolset to shape the resulting sound in a musical way. Each block size channel has its own spectrum shift and freeze section (based on the phase-locked vocoder). A spectral filter implemented with a cepstrum analysis is available at the end of the signal path.
More info: [DBS](https://sites.google.com/site/bilberry79/)
![alt text](https://github.com/bilberry79/PureData/blob/master/pictures/DBS.PNG)

<h3>Discrete summation formula (DSF) adapted from Moorer 1975</h3>
In "The Synthesis of Complex Audio Spectra by Means of Discrete Summation Formulae" from 1975, Moorer presents 4 different ways of creating complex spectra.

`[dsf1fin~]`: 1-sided finite spectrum.

`[dsf1infin~]`: 1-sided infinite spectrum.

`[dsf2fin~]`: 2-sided finite spectrum.

`[dsf2infin~]`: 2-sided infinite spectrum.
