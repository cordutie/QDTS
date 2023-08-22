## Example 2 - Masking

Example 2 consists of the synthesis of a single pitch overlapped with filtered noise. 
The audio example contains the single pitch synthesized using additive synthesis and **QDTS** 
synthesis first and then overlaps it with a high-passed filtered noise. The effect of the
filtered noise with the synthesized pitch using additive synthesis is simply hearing both sounds, 
however, when the filtered noise is played together with the **QDTS** synthesis, 
the synthesized pitch gets muted because of the disorder around the _carrier_
complex of pure tones.

For the **QDTS** synthesis, the computations were made using the `qdts.solver` 
object using a _carrier_ complex of pure tones with C=2338Hz in order to 
synthesize a single pitch with frequency F=55Hz and a particular harmonic distribution. 
The noise was filtered muting all frequencies below approximately 1100Hz.
