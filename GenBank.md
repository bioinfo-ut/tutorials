### GenBank 'Accession number'i järgi järjestuste allalaadimine
```
module load edirect
esearch -db nucleotide -query KC170303 | efetch -format fasta > KC170303.fasta
```

### Metainfo pärimine
```
module load edirect
epost -db nuccore -id KC170303 | esummary | xtract -pattern DocumentSummary -element TaxId,Organism,AccessionVersion,Title
```
