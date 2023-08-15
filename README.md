# QDTS

Quadratic Difference Tone Spectra (QDTS) is a particular kind of
auditory distortion product where several sinusoids are combined
to generate a full spectra of quadratic difference tones (QDT). 
This repository contains an implementation as a MAX external of 
the algorithm built to generate QDTS presented at the International 
Computer Music Conference 2023 hosted in the Chinese University of 
Hong Kong.

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