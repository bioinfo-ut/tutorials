## Conda
Condaga saab luua virtuaalkeskkondi kuhu saab installida mooduleid ja vajalikke pythoni versioone ilma rooti õiguseta.
Conda pole ainult pythoni-keskne ja läbi selle saab kasutada `npm`-i ja installida R-i pakette(?)

## Conda kasutamine mambas
Pathis condat pole seega tuleb iga kord laadida python, kus see on olemas:
```
module load python-3.6.3
```
**NB! Kuigi laetud sai kindel versioon pythonist, saab keskkondi luua suvalise(?) pythoni versiooniga.**

### Keskkonna loomine:
```
conda create --name my_env python=3.8
```
pythoni versiooni lisamine on valikuline, antud näites luuakse keskkond versiooniga 3.8, mida pole mambas ega moodulite all

### Keskkonna aktiveerimine 
```
source activate my_env
#conda activate my_env
```
Mambas on vanem conda - kasutada esimest rida, uuematega kasutatakse teist

### Moodulite installimine 
```
conda install -c conda-forge -c bioconda sourmash
```
Lisatakse moodulid `bioconda` ja `sourmash`
### Keskonna loomine yml faili järgi
```
conda env create -f my_yml.yml
```
### Olemasolevad keskkonnad
```
conda env list
```
### Keskkonna kustutamine
```
conda env remove -n my_env
```
