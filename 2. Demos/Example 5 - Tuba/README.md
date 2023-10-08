## Example 5 - Tuba

Example 5 consists of the resynthesis of a real recording of a tuba through **QDTS** synthesis. The audio example contains 
the real tuba recording, a resynthesis of the real recording using a combination of 8 sinusoids with a pitch detector, 
a combination of the resynthesis made with the 8 sinusoids and with the **QDTS** synthesis, the combination of the real 
recording with the resynthesis using **QDTS** synthesis versions, and finally the resynthesis using **QDTS** synthesis alone. 
The results show that certain signals can be at a certain level be reconstructed using **QDTS** synthesis.

For the **QDTS** synthesis, the computations were made using the `qdts.solver` object using a _carrier_ complex 
of pure tones with C=1979Hz in order to resynthesize the recording of a tuba (see note below). The harmonic distribution 
was precomputed using the Discrete Fourier Transform of a small bin of the real recording. The pitch and envelope detection 
of the tuba recording were made in real-time using the `sigmund` object. Finally, the square root of the envelope of the 
real signal was used in the **QDTS** synthesis as in Example 3.

>Note: the recording of the tuba was downloaded from [here](https://freesound.org/people/josemdavid/sounds/406607/).

[![Alt text](https://i3.ytimg.com/vi/UodLZ9XQ_S0/maxresdefault.jpg)](https://youtu.be/UodLZ9XQ_S0)
