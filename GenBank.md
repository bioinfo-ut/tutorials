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
### Edirect tööriistad:
https://www.ncbi.nlm.nih.gov/books/NBK179288/

Muuhulgas on võimalik teha ka päringuid Pubmedi

### Accession numbers
https://www.ncbi.nlm.nih.gov/Sequin/acc.html
https://www.ncbi.nlm.nih.gov/books/NBK21091/table/ch18.T.refseq_accession_numbers_and_mole/
