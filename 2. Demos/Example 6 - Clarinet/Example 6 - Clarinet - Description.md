## Example 6 - Clarinet

> Disclaimer: before start describing this example, it is important to mention that here we are resynthesizing a much higher in pitch
signal than in the previous example, and hence to hear this Auditory Distortion Products it is required to increase the 
volume of the loudspeakers used.

Example 6 consists of the resynthesis of a real clarinet recording (see note below) through various Auditory Distortion Products. The audio 
example contains the real clarinet recording followed by three resynthesis of it using three different **QDTS** synthesis settings. 
The results show that the same signal can be recreated using different **QDTS** synthesis settings allowing to have at least some 
control on the timbre of the _carrier_ complex of pure tones.

For the **QDTS** synthesis, the computations were made using the `qdts.solver` object using a _carrier_ complex 
of pure tones with $C=2345$Hz. The computations were ran several times until three reasonably different solutions appeared. 
The harmonic distribution was precomputed using the Discrete Fourier Transform of a small bin of the real recording. 
The pitch and envelope detection of the tuba recording were made in real-time using the `sigmund` object. Finally, 
the square root of the envelope of the real signal was used in the **QDTS** synthesis as in Example 3.

>Note: the recording of the tuba was downloaded from [here](https://freesound.org/people/stephenchai/sounds/20932/). 