# Transcriptomic Parcellation of the Cortex

Parcellation of the Human Cortax based on gene expression. This projects uses data from the Allen Institute for Brain Science.
More precisely: https://human.brain-map.org/.

After selecting about 1221 probes that sample cortical gene expression in the left hemisphere (see here for pre-processing and probe selection: https://github.com/andrealtmann/AIBS_FTD).
Principal components of gene expression are extracted and interpolated across the entire cortex (see here for related code: https://github.com/andrealtmann/gene2surface).
This results in a map with 22 gene expression principal components for each of the ~10,000 nodes in the fsaverage5 suface.
Finally, hierachical clustering with complete linkage is used to parcellate the cortex; we cut the tree to optain 10, 25, 50, or 100 clusters. 
The maps are available as annotation files for fsaverage5.

For more details see the poster presented at OHBM2020 here: http://altmann.eu/documents/posters/OHBM2020_Altmann_transcriptomics.pdf
