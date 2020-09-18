## MAMBA kettad
MAMBAs on ca 300 TB kettaruumi.
See ruum on jagatud loogilisteks ketasteks, millest peamised on:
> /mambakodu  
> /storage5  
> /storage6  
> /storage7  
> /storage8  
> /storage9  
> /storage10  
> /smallea  
> /bigea

***/mambakodu*** on 3.7 TB suurune ketas, mille peal asuvad kõigi kasutajate kodukataloogid.
Oluline on jälgida, et te ei kirjutaks oma kodukataloogi servani täis. Kui /mambakodu on 100% täis, siis ei saa ükski kasutaja enam MAMBAsse sisse logida.   
MAMBA koduketta täituvust on võimalik jälgida käsuga:
> $df -h /mambakodu  
> Filesystem          Size  Used Avail Use% Mounted on  
> /dev/mapper/mpathb1 3.7T  2.7T 1010G  73% /mambakodu

***/storage5 kuni /storage10*** on 50TB suurused kettad, mis mõeldud suuremahuliste andmete hoidmiseks. Igal kettal on vastutav isik, kes hoolitseb, et vastaval kettal oleks piisavalt ruumi, tekitab sinna sobiva failistruktuuri ja otsustab kes ja mida sellel kettal hoiab.  
Vastutajad on:  
/storage5 Lauris  
/storage6 varus  
/storage7 Tarmo  
/storage8 Triinu  
/storage9 Reidar  
/storage10 Maido  

Kõik suuremahulised kirjutamised /storage ketastele palun kooskõlastada ketta haldajaga!


***/smallea (750 GB) ja /bigea (2 TB)*** on SSD kettad, mis mõeldud ketta-intensiivsete arvutuste läbiviimiseks. Mõned arvutused on tunduvalt kiiremad kui kasutada SSD kettalt lugemist. Mõlemad kettad on mõeldud ainult **ajutiseks** andmete hoidmiseks. Teie failid võidakse sealt igal hetkel kustutada.

## Varundamine
Ketastel olev info varundatakse igal öösel lintidele HPC keskuse töötajate poolt. Failide taastamiseks pöörduda serveri haldajate poole aadressil support@hpc.ut.ee  
