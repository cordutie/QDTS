## Example 3 - AM

Example 3 consists of the synthesis of an amplitude-modulated single pitch. 
The audio example contains the amplitude-modulated pitch synthesized using 
additive synthesis, the combination of the additive and **QDTS** synthesis versions, 
and the **QDTS** synthesis alone for comparison. It is important to note that since 
the Quadratic Tones arise from the Distortion function $D=(d_1,\dots,d_{n-1})$ 
and such function is homogeneous of degree $2$ one has that

$$D(\lambda x)=\lambda^2 D(x),$$

so in order to apply amplitude modulation, one has to use the square root 
of the usual AM _carrier_.

For the **QDTS** synthesis, the computations were made using the `qdts.solver` 
object using a _carrier_ complex of pure tones with $C=2338$Hz in order to 
synthesize a single pitch with frequency $F=55$Hz and a particular harmonic distribution. 
The AM _carrier_ used was a simple LFO of the form 

$$L_1(t)=A\sin(\omega t+\varphi)+B,$$

for some $A,B,\omega,\varphi\in\mathbb{R}$ in the additive synthesis case, and the squared 
root version of the LFO 

$$L_2(t)=\sqrt{A\sin(\omega t+\varphi)+B},$$

for its **QDTS** counterpart. 