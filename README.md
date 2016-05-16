# PureData
PureDate patches and abstracts

<h3>Audio analyzer</h3>
`abstract_lin_spec_2.pd`

A tool to visualize the frequency spectrum and the wave form of two audio inputs. 
![alt text](https://github.com/bilberry79/PureData/blob/master/pictures/abstract_lin_spec_2.PNG)

`abstract_spec.pd`

A tool to visualize the frequency spectrum in a logarithmic and linear view of one audio input. 

<h3>Dynamic Block Switching Synthesis</h3>
`DBS.pd`

This tool proposes a new sound synthesis algorithm based on dynamic block switching techniques used in common MP3 compression. After the transformation of the analysis signal in the frequency domain (STFT), a transient detection algorithm triggers the block switching decisions that synthesize a new sound. Block sizes of 128-8192 samples are possible. Smaller block sizes assure a more precise localisation of the audio event in time and larger block sizes smear the onset of an event in time but provide a richer overtone spectrum. Several spectral effects are available to give the user a broad toolset to shape the resulting sound in a musical way. Each block size channel has its own spectrum shift and freeze section (based on the phase-locked vocoder). A spectral filter implemented with a cepstrum analysis is available at the end of the signal path.
More info: [DBS](https://sites.google.com/site/bilberry79/)
![alt text](https://github.com/bilberry79/PureData/blob/master/pictures/DBS.PNG)
