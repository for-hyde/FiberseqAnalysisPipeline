# FiberseqAnalysisPipeline
A snakemake analysis pipeline using Snakemake for the alignment and analysis of Fiberseq data. 

# How to use
First, you will need your unaligned BAM file. There are two options: copy your files to the resources folder or define your own files in the config/config.yaml file. 
Along with the BAM file you will need the reference genome. Finally, you will need the 

## Running on a cluster with SLURM submission 
In the profiles folder are two folders: a default and a SLURM based one. The default folder is for the parameters to run the analyis locally. To use the SLURM config file you must first adjust the values to match your profile and partition on the HPC environment. The alignment portion is computationally expensive as is the generation of the pileup files.
