# Wang_dataset

![flr](https://user-images.githubusercontent.com/2476893/213655687-96ea44ae-ea61-4be2-b979-8dd47e72e7c4.png)

Dataset of "Accurate and Reliable Prediction of Relative Ligand Binding Potency in Prospective Drug Discovery by Way of a Modern Free-Energy Calculation Protocol and Force Field" (J. Am. Chem. Soc. 2015, 137, 7, 2695–2703) https://pubs.acs.org/doi/10.1021/ja512751q

すべてのPDBおよび化合物・中間体の情報は、Assessment of Binding Affinity via Alchemical Free-Energy Calculations (J. Chem. Inf. Model. 2020, 60, 6, 3120–3130)
https://pubs.acs.org/doi/abs/10.1021/acs.jcim.0c00165 で用いられたCresset Flare FEPプロジェクトファイルからdata exportすることで取得した。

-----

`dataset/dataset_mid_ligands.sdf`にはFlare FEPで中間体として導入されたリガンドが含まれる。
中間体には仮名及び導入された中間体がFlare FEPで導入されたときにリンクしていた化合物の名称を複合した名称を用いた。`dataset/complex/`内には仮名のみが用いられる。
`wibble;CAT-13a_mk1`、`mk1;CAT-13f_CAT-13d_CAT-13o_CAT-13a_CAT-13g_CAT-13e_mk2_mk3_wibble`とすることで、仮名称に対してリンクしていることを示した。


JNK1とThrombinは中間体が導入されなかったため、`dataset/dataset_mid_ligands.sdf`はファイルは存在しない。



`dataset/complex/` には各リガンドの複合体poseにおける座標情報 (PDB) が含まれる。ターゲットのPDBと重ねることでシミュレーションの初期構造となる複合体構造PDBになる。
