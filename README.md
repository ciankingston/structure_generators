# structure_generators

There are a number of published methods for the generation of biologically relevant molecules/analogs

(1) mmpa_medchem_playbook.ipynb

This script generates analogs using medicinal chemistry "intuition" which is obtained via matched molecule pair analysis of the ChEMBL database.The workflow is described in J. Chem. Inf. Model. 2021, 61, 2, 729 (https://pubs.acs.org/doi/10.1021/acs.jcim.0c01143 and an overview of the code is available at https://github.com/mahendra-awale/medchem_moves). Note mmpdb v2.2 was required, which was directly installed from github (pip install git+https://github.com/mahendra-awale/medchem_moves.git). This package requires the chemblDB3.sqlitdb to be downloaded and stored.

(2) user_defined_molecular_assembly.ipynb + amines.xlsx + BAs.xlsx

This script assembles molecules using user-defined fragments. In the example, the chosen molecular core bears a bromide and a carboxylic acid. The bromide will be used in a Suzuki reaction while the acid will be used for amide coupling. The 150 possible products from user-defined lists of 15 boronic acids and 10 amines are virtually synthesized. Molecular descriptors are generated and the molecules are clustered to provide a representative set. Code adapted from: https://greglandrum.github.io/rdkit-blog/tutorial/rgd/2022/03/14/rgd-and-molzip.html

(3) crem.ipynb

