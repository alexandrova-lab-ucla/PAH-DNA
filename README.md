# PAH-DNA
Genotoxicity of PAH-DNA adducts 

Nanoscale Molecular Dynamics (NAMD) and Visual Molecular Dynamics (VMD) software is used to run molecular dynamics simulations and free energy perturbations.

User guides:\
NAMD: [Unix/Mac](http://www.ks.uiuc.edu/Training/Tutorials/namd/namd-tutorial-unix.pdf) or [Windows](http://www.ks.uiuc.edu/Training/Tutorials/namd/namd-tutorial-win.pdf)\
[VMD](http://www.ks.uiuc.edu/Training/Tutorials/vmd/vmd-tutorial.pdf)

## File Explanations: <br />
### equil_scripts <br />
These scripts are needed for preparation of the system to undergo simulations. <br /> The order is significant. <br />

1) Minimize the system to ensure reasonable atom positions <br />
file: min2.namd <br />

2) Relax the backbone and water box in the system, while also maintaining shape. <br />
file 1: equilNVT2.namd <br />
file 2: equilNPT2.namd <br />

3) Shape water box for most stable box possible, minimizing surface tension <br />
file: equilibrate_IA2.namd <br />

4) Run FEP forwards and backwards. <br />
file 1: forward_IA-on3.namd <br />
file 2: backward_IA-on3.namd <br />


Toppar\
Topology files defining bonds between atoms. 

**README and this repository are still in progress.**
