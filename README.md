# APARM
Software for obtaining association parameters from a supramolecular system (ACS Omega 5, 5013–5025, 2020).

1.	Introduction
The APARM software reads a XYZ file that contains a supramolecular system. 
To run APARM, you have to use the following files:
aparm-GEOMETRY.xyz
aparm.inp.xyz

aparm-GEOMETRY.xyz : a file that contains the XYZ cartesian coordinates (with atomic number or symbol) of the supramolecular system. The first set of coordinates MUST corresponds to the smaller molecule and the second set, to the bigger system or the reference system. 
ud-aparm-MOLECULE_2-REFERENCE.xyz: a file that contains the XYZ Cartesian coordinates of the fixed in space molecule (usually the greater molecule in a supramolecular system).
aparm.inp: a file that contains three lines (with total number of atoms, atoms of the smaller molecule and atoms of the reference molecule). 

2.	Installation
The pre-compiled Linux APARM file ("aparm-linux") can be downloaded from https://github.com/anconi-lab/APARM. 
After creation of the directory "/home/aparm" in your linux distro, into .bashrc ncludes the following line:
alias aparm='/home/aparm/aparm-linux'
After editing such a file, download run-test-aparm.tar.gz and extract the files: 
>tar  -xzvf run-test-aparm.tar.gz
At run-test-aparm , run APARM to test
>./aparm-linux
With UCSF Chimera installed, you can see the supramolecular systems and vectors that define the relative position between the molecules (.bild files). 
The parameters for supramolecular characterization are discussed in the following publication:
Relative Position and Relative Rotation in Supramolecular Systems through the Analysis of the Principal Axes of Inertia: Ferrocene/Cucurbit[7]uril and Ferrocenyl Azide/β-Cyclodextrin Case Studies. ACS Omega 2020, 5, 10, 5013–5025. 



3.	APARM input
APARM input consists of three lines. The first line contains the total number of atoms of the supramolecular system, the second line the number of the atoms of the small molecule, and the third with the number of atoms of the reference and fixed molecule. 

4.	How to cite and License
The ideas related to the implementation are descr¬ibed in the contribution published in ACS Omega (Cleber P. A. Anconi, ACS Omega 2020, 5, 5013 – 5025). The codes were improved and revised since the publication. Therefore, the version employed in your work should be identified. For reproducibility, the present version does not handle high symmetric molecules, such as benzene. The multiple possible values for the supramolecular parameters for highly symmetric systems are under investigation. 

LICENSE INFORMATION: To download and use APARM, you are required to read and agree to the following terms:
(a) Currently, APARM is free of charge for academic and commercial usage. Anyone can freely distribute the original or their improved versions to others.
(b) APARM can be distributed as a free component of commercial code. 
(c) APARM is utilized in your work. The original ACS Omega paper MUST BE cited in your work (with the version of the software used): 
Anconi, C. P. A.  ACS Omega 2020, 5, 5013 – 5025. APARM, version 1.22. 
(d) There is no warranty of the correctness of the results produced by APARM. The author does not hold responsibility in any way for any consequences arising from the use of the APARM software.
