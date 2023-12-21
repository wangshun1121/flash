# FLASH from JHU

## About FLASH

[FLASH](http://ccb.jhu.edu/software/FLASH/index.shtml) (Fast Length Adjustment of SHort reads) is a very fast and accurate software tool to merge paired-end reads from next-generation sequencing experiments. FLASH is designed to merge pairs of reads when the original DNA fragments are shorter than twice the length of reads. The resulting longer reads can significantly improve genome assemblies. They can also improve transcriptome assembly when FLASH is used to merge RNA-seq data.

## About this release

I slightly modified the quality value calculation method based on FLASH v1.2.11. Source code can be downloaded [here](http://ccb.jhu.edu/software/FLASH/FLASH-1.2.11.tar.gz), and it is the initial commit of this repository. 

For common bases in combined reads, quality scores of consensus bases were chosen from higher values of due paired reads in original code. I use the sum of both quality value as consensus Q value.