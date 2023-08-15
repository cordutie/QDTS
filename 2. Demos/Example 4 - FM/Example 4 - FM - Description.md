## Example 4 - FM

Example 4 consists of the synthesis of a frequency-modulated single pitch. 
The audio example contains the frequency-modulated pitch synthesized using 
additive synthesis, the combination of the additive and **QDTS** synthesis versions, 
the **QDTS** synthesis alone, and a **QDTS** synthesis using frequency modulation on the 
_carrier_ instead of the _target_ for comparison. The result shows 
that frequency modulation is compatible with **QDTS** synthesis in certain ranges. 
Moreover, when the _carrier_ complex of pure tones is frequency modulated, 
the auditory distortion product holds its pitch, since the difference of the 
frequencies of the _carrier_ complex of pure tones holds the same, however, 
some amplitude changes can be heard in this case, showing the instability of the 
auditory distortion products with respect to the _carrier_ frequencies.

For the **QDTS** synthesis, the computations were made using the `qdts.solver` 
object using a _carrier_ complex of pure tones with $C=2500$Hz in order to 
synthesize a single pitch with frequency $F=55$Hz and a particular harmonic distribution. 
The FM _carrier_ used was a simple LFO of the form 

$$L(t)=A\sin(\omega t+\varphi)+B,$$ 

for some $A,B,\omega,\varphi\in\mathbb{R}$ in both the additive and **QDTS** synthesis case.