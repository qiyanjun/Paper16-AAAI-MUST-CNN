# MUST-CNN

Code for the paper "MUST-CNN:	A	Multilayer	Shift-and-Stitch	Deep	Convolutional	Architecture	for	Sequence-Based Protein	Structure	Prediction" (AAAI 2016)



# Requirements
Code is written in Lua and requires [Torch] (http://torch.ch/). Running on the GPU via the cuda cunn library is strongly reccommended (use the -cuda parameter). To get cunn, use:
``
luarocks install cunn
``

# Data
The data is split up into 3 directories: 4Protein, 28 Protein, and cb513. Each directory contains a "data" subdirectory and a "hash" subdirectory. The data subdirectory contains "aa1.dat" which is the raw protein sequence data, as well as each *tag.dat file which are the class labels for each separate class. The data subdir also contains the psi-blast files. The hash subdirectory contains the dictionary numbers for each of the amino acids and class labels.

# Running the code
The code should be runnable with the default parameters by simply executing ``th main.lua``. See cmdlineargs.lua to pass in parameters.
