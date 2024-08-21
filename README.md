# Wang-FEP-dataset

![flr](https://user-images.githubusercontent.com/2476893/213655687-96ea44ae-ea61-4be2-b979-8dd47e72e7c4.png)

Dataset of "Accurate and Reliable Prediction of Relative Ligand Binding Potency in Prospective Drug Discovery by Way of a Modern Free-Energy Calculation Protocol and Force Field" (J. Am. Chem. Soc. 2015, 137, 7, 2695–2703) https://pubs.acs.org/doi/10.1021/ja512751q

All PDB and compound/intermediate information was obtained by exporting data from the [Cresset Flare FEP project file](https://drive.google.com/file/d/1dIaSZ5J4GdHXNdrtPBVdLfJYdsxOuHb2/view?usp=sharing) used in the "Assessment of Binding Affinity via Alchemical Free-Energy Calculations" (J. Chem. Inf. Model. 2020, 60, 6, 3120–3130) https://pubs.acs.org/doi/abs/10.1021/acs.jcim.0c00165.

The file `dataset/dataset_mid_ligands.sdf` contains ligands introduced as intermediates in Flare FEP. The intermediates are named by combining a pseudonym with the compound's name to which the intermediate was linked when introduced in Flare FEP. In the directory `dataset/complex/`, only pseudonyms are used. For example, `wibble;CAT-13a_mk1` or `mk1;CAT-13f_CAT-13d_CAT-13o_CAT-13a_CAT-13g_CAT-13e_mk2_mk3_wibble` indicates that the pseudonym is linked to the respective compounds.

Since intermediates were not introduced for JNK1 and Thrombin, the file `dataset/dataset_mid_ligands.sdf` does not exist.

The `dataset/complex/` directory contains the coordinate information (PDB) of each ligand's complex pose. By superimposing this onto the target's PDB, you obtain the complex structure PDB, which is the initial structure for simulations.
