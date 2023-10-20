<div align="center">
  
# QDTS

[**Rodrigo Cádiz**](https://rodrigocadiz.com/music/)<sup>1,2</sup>, [**Esteban Gutiérrez**](https://github.com/cordutie)<sup>3</sup>, and [**Christopher Haworth**](https://www.birmingham.ac.uk/staff/profiles/music/haworth-christopher.aspx)<sup>4</sup>

<sup>1</sup> *Music Institute, Pontificia Universidad Católica de Chile* <br>
<sup>2</sup> *Department of Electrical Enginering, Pontificia Universidad Católica de Chile* <br>
<sup>3</sup> *Department of Information and Communications Technologies, Universitat Pompeu Fabra* <br>
<sup>4</sup> *Department of Music, University of Birmingham* <br>

<div align="left">

## Introduction

Cuadratic and cubic difference tones (QDT and CDT respectively) are
a particular kind of auditory distortion products (ADP) where two 
pure tones are used to generate the perceptual illusion of a third 
pure tone. This ADPs have been thoroughly studied and compared in the
last decades (see e.g. [[1]](#1), [[2]](#2) and [[3]](#3)),
and the necessary conditions to generate them are well known.
Quadratic Difference Tone Spectra (QDTS) on the other side, is a 
new kind of ADP where several pure tones are combined to generate a 
full spectra made out of QDT.

The theory behind the construction of a QDTS was first introduced in 
[[4]](#4), and a real-time algorithm that solves the computations
needed to generate any given QDTS was first introduced in [[5]](#5).

This repository contains an implementation as a MAX external of 
the algorithm built in [[5]](#5) to generate QDTS presented at the 
International Computer Music Conference 2023 hosted in the Chinese 
University of Hong Kong.

[![Alt text](https://i3.ytimg.com/vi/UodLZ9XQ_S0/maxresdefault.jpg)](https://youtu.be/UodLZ9XQ_S0)

## Contents

The three main folders of the repository contain the implementation
in MAX, some example patches recorded in video and the experiments
that supported the contruction of the algorithm itself respectively.

### 1. MAX external

In this folder everything related to the MAX external can be found.

- The subfolder **Builds** contains current builds for the external
for the Windows and MAC operative systems. A little tutorial on how
to run the external can also be found in this subfolder.

- The subfolder **Code** contains the necessary code to build the MAX
external in case that the current builds stopped working. A little
tutorial on how to build the MAX external can also be found in this
subfolder.

- The subfolder **Patches** contains several MAX files that can be used 
to easily manipulate the MAX external. 

### 2. Demos

In this folder, several video demos of the MAX external. Each demo 
contains a brief readme file containing a description of it, an 
uncompressed audio file of the demo and a series of patches to recreate
the video demo locally.

### 3. Experiments

The algorithm implemented uses several standard mathematical tools,
however due to its heuristic nature, several experiments were made 
prior to its construction in order to fully understand the problem.

In each subfolder, a python project containing the experiment can be
found together with a brief readme file containing a description of
the experiment itself.  

## References

<a id="1">[1]</a> J. B. Dewey, “Cubic and quadratic distortion products in vibrations of the mouse cochlear apex,” JASA Express Letters 2, vol. 11, no. 114402, 2022.\
<a id="2">[2]</a> E. Zwicker, “Different behaviour of quadratic and cubic difference tones,” Hearing Research, vol. 1, no. 4, pp. 283–292, 1979.\
<a id="3">[3]</a> R. Plomp, “Detectability threshold for combination tones,” The Journal of the Acoustical Society of America, vol. 37, no. 1110, 1965.\
<a id="4">[4]</a> G. Kendall, C. Haworth, and R. F. Cádiz, “Sound synthesis with auditory distortion products,” Computer Music Journal, vol. 38, no. 4, 2014.\
<a id="5">[5]</a> C. Haworth, E. Gutiérrez and R. F. Cádiz, “Generating Quadratic Difference Tone Spectra for Auditory Distortion Synthesis,” (to be published).
