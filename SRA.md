# Sequence Read Archive (SRA)
https://www.ncbi.nlm.nih.gov/sra  
TODO: Sequence Read Archive (SRA) data, available through multiple cloud providers and NCBI servers, is the largest publicly available repository of high throughput sequencing data. The archive accepts data from all branches of life as well as metagenomic and environmental surveys. SRA stores raw sequencing data and alignment information to enhance reproducibility and facilitate new discoveries through data analysis.

## Järjestuste allalaadimine
```
module load sra-toolkit-2.8.2
fastq-dump SRR5070677
```
NB! Moodulite all olev 2.8.2 on vanem versioon. Uuema versiooni all on `fasterq-dump`, mis on kiirem.  
TODO: uuri Tarmolt/Reidarilt, kuidas saab veel kiiremini alla laadida kasutades `prefetch` vaheetappi.

## Metainfo allalaadimine
Väljund: STDOUT
```
module load edirect
esearch -db sra -query SRR5070677 | efetch -format runinfo
```
