# Neutron_Star_EOS

== Table of Content ==

0. Codes and input files that produe the EoSs
1. Correspondence between EoS folders and paper figures
2. Files in the folders
3. Neutron star observation constraints


==== 0. Codes and input files that produe the EoSs ========================================================

To run the code, one requires the folder input_files, the Mathematica code, and a generic folder called output_files and output_files/TW (the generated EoS will be outputed here).  We have also uploaded the EoS folders as well but those are the output of the code and not required to run the code.

We include two different codes here, please cite the following papers:<br>
PRL_EOS_TOV.nb: Tan, Noronha-Hostler, Yunes, Phys.Rev.Lett. 125 (2020) 26, 261104 <br>
PRD_Twins_TOV.nb: Tan, Dore, Dexheimer, Noronha-Hostler, Yunes to appear<br>



If the SLy crust was used cite:<br>
E. Chabanat, P. Bonche, P. Haensel, J. Meyer, and R. Schaef-fer.   A  Skyrme  parametrization  from  subnuclear  to  neutronstar  densities.  2.  Nuclei  far  from  stablities.Nucl.  Phys.  A,635:231–256,  1998.   [Erratum:  Nucl.Phys.A  643,  441–441(1998)].doi:10.1016/S0375-9474(98)00180-8<br>
F. Douchin and P. Haensel.   Inner edge of neutron star crustwith SLY effective nucleon-nucleon interactions.Phys. Lett.B,  485:107–114,  2000.arXiv:astro-ph/0006135,doi:10.1016/S0370-2693(00)00672-9.<br>
F.  Douchin  and  P.  Haensel.   A  unified  equation  of  state  ofdense matter and neutron star structure.Astron. Astrophys.,380:151, 2001.arXiv:astro-ph/0111092,doi:10.1051/0004-6361:20011402.<br>
F  Douchin,  P  Haensel,  and  J  Meyer.    Nuclear  surface  andcurvature properties for SLy Skyrme forces and nuclei in theinner neutron-star crust.Nucl. Phys. A, 665:419–446, 2000.<br>


==== 1. Correspondence between EoS folders and paper figures ========================================================
Fig.4 top    -> /adjustedwidth<br>
Fig.4 bottom -> /peaklocation<br>
Fig.5        -> /endpoint<br>
Fig.6        -> /2bumpsfat<br>

Fig.7   blue dotted dash -> /crust/QHC-125<br>
	red dash	 -> /endpoint_maxfull/eos3<br>
	green solid	 -> /crust/SKA-140<br>
	blue dash        -> /crust/QHC-275<br>
	red solid        -> /endpoint_maxfull/eos1<br>
	green dash       -> /crust/SKA-300<br>

Fig.8        -> /endpoint_maxfull<br>

Fig.9   blue dash  ->      /peaklocation/eos1<br>
	pink solid ->      /endpoint_maxFull/eos2<br>
	red dotted-dash -> /endpoint_maxfull/eos3<br>
	cyan solid ->      /slanted_3M/eos1<br>
	green dash ->      /endpoint_3M/eos4<br>
	megenta solid ->   /2bumpsfat/eos1<br>

Fig.11  purple dash -> TW/peakwide_longcs0/eos4<br>
	brown dotted-dash -> TW/peakwide_longcs0/eos2<br>
	blue solid -> TW/highhyb/eos1<br>
	green dash -> TW/peakwidthFIXL/eos1<br>

 
Fig.12  blue dotted dash -> /TW/Blat_repeat/eos1<br>
	red solid        -> /TW/Blat_repeat/eos3<br>
	green dash       -> /TW/low_n_peak1st/eos2<br>


Fig.13       -> /TW/peakwidthFIXL<br>

Fig.14  purple dash       -> /TW/pickFIX_PTwidth/eos1<br>
	deep green dash   -> /TW/pickFIX_PTwidth/eos2<br>
	light green dash  -> /TW/pickFIX_PTwidth/eos3<br>
	blue dot          -> /TW/pickFIX_PTwidth/eos4<br>
	black solid       -> /TW/pickFIX_PTwidth2/eos1<br>
	brown dotted dash -> /TW/pickFIX_PTwidth2/eos3<br>
	brown dash        -> /TW/pickFIX_PTwidth3/eos4<br>

Fig.15       -> /TW/slantendpoint<br>
Fig.16       -> /TW/endpoint<br>

==== 2. Files in the folders =================================================================================

In each folder, there should be at least 3 types of files: EoS, mr, all observables


For EoS, the file name is eosX.dat, where X is a number.<br>
There are five columns in eosX.dat, which are <br>
baryon density[1/fm^3], pressure[MeV/fm^3], energy density[MeV/fm^3], speed of sound squared[], chemical potential[MeV]<br>


For mr, the file name is mrX.dat, where X is a number.<br>
There are four columns in mrX.dat; the first three of them are:<br>
radius of NS[km], mass of NS[solar mass], central energy density[MeV/fm^2]<br>


For files contain all observables, the file name is eosX_CntDens[MeV]_R[km]_M[Msun]_Ibar_Qbar_Love.dat<br>
There are 6 columns in the files, which are<br>
center energy density, radius of NS, mass of NS, dimensionless moment of inertia, dimensionless quadrupole moment, dimensionless Love number.<br>
The units are shown in the filenames, where MeV really means MeV/fm^3 and Msun means solar mass.<br>


==== 3. Neutron Star observation constraints ==================================================================

GW170817:<br>
	publication: http://arxiv.org/abs/1805.11581<br>
	repository: https://dcc.ligo.org/LIGO-P1800115/public<br>

GW190814:<br>
	publication: http://arxiv.org/abs/2006.12611<br>

J0030+0451 Illinois-Maryland:<br>
	publication: http://arxiv.org/abs/1912.05705<br>
	repository: https://zenodo.org/record/3473466#.YMDjgTZKidY<br>

J0030+0451 Amsterdam:<br>
        publication: https://arxiv.org/abs/1912.05702<br>
        repository: https://zenodo.org/record/3386449#.YMDkDjZKidY<br>

J0740+6620 Illinois-Maryland:<br>
	publication: https://arxiv.org/abs/2105.06979<br>
	repository: https://zenodo.org/record/4670689#.YMDmSjZKidY<br>

J0740+6620 Amsterdam:<br>
        publication: https://arxiv.org/abs/2105.06980<br>
        repository: https://zenodo.org/record/4697625#.YMDlZjZKidY<br>

V723 Mon: <br>
	publication: https://arxiv.org/abs/2101.02212<br>




