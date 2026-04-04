# Kuidas kirjutada head dokumentatsiooni

## Lühike versioon

Dokumentatsioon on tehniline tõendusmaterjal, mitte lihtsalt samm-sammuline juhend või ekraanipiltide kogumik. 
Dokumentatsioon kirjutatakse umbisikulises vormis (tehti, paigaldati, muudeti), mitte "mina tegin".

See peab vastama kolmele küsimusele:
- mida tehti  
- miks tehti  
- milline on tulemus  

Näide:
- paigaldati tarkvara käsuga `sudo apt install pakett`, et võimaldada teenuse käivitamine ja edasine seadistamine
- [näiteks tõestus pildina]

Tulemus peab olema tõendatav:
- käsu väljund  
- logi või päringu tulemus  
- ekraanipilt  
- link (kui see viib otseselt kontrollitava tulemuseni)  

Käsud ja kood tuleb eraldi ja selgelt vormindada. Dokumentatsiooni põhjal peab olema võimalik tehtut kontrollida.

## Pikk versioon

Dokumentatsiooni eesmärk on tõendada tehtud tööd. See ei ole lihtsalt tegevuste kirjeldus, vaid selgitus, mis näitab, et autor saab aru, mida ta teeb ja suudab tulemust põhjendada.

## 1. Mida tehti

Kirjelda konkreetselt tehtud tegevused.

Väldi üldsõnalisi lauseid:
- “seadistasin süsteemi”
- “tegin vajalikud muudatused”

Too välja:
- millised tegevused tehti  
- milliseid käske või tööriistu kasutati  

Näide (halb):
- seadistasin serveri

Näide (hea):
- paigaldati vajalik tarkvara käsuga `sudo apt install pakett`

## 2. Miks tehti

Iga oluline tegevus peab olema põhjendatud.

Näita:
- miks see samm oli vajalik  
- mida see muudatus lahendab või mõjutab  

Näide (halb):
- muudeti seadistust

Näide (hea):
- seadistust muudeti, et piirata ligipääsu ainult lokaalsele masinale

## 3. Milline on tulemus

Dokumentatsioon peab näitama lõpptulemust.

See tähendab:
- kuidas kontrolliti, et asi töötab  
- milline oli kontrolli tulemus  

Näide (halb):
- süsteem töötab

Näide (hea):
- kontrolliti teenuse olekut käsuga `systemctl status teenus`  
- väljund näitas: active (running)

## 4. Vormistus ja kirjutamisviis

Dokumentatsioon kirjutatakse **umbisikulises vormis**.

See tähendab:
- kasutatakse: tehti, paigaldati, muudeti  
- ei kasutata: ma tegin, ma paigaldasin  

Näide (halb):
- ma paigaldasin tarkvara  
- ma muutsin faili  

Näide (hea):
- tarkvara paigaldati  
- konfiguratsioonifaili muudeti  

Käsud ja kood tuleb esitada kas:
- eraldi koodiplokis (pikemad käsud)  
- või rea sees (lühemad käsud)

## 5. Väldi tüüpvigu

Halb dokumentatsioon:

- kirjeldab ainult tegevust, mitte tulemust  
- ei põhjenda tehtud samme  
- kasutab üldsõnalisi väljendeid  
- sisaldab pilte ilma selgituseta  

Hea dokumentatsioon:

- on konkreetne  
- on põhjendatud  
- on kontrollitav  

## Kokkuvõte

Hea dokumentatsioon:

- näitab tehtud tööd  
- selgitab otsuseid  
- tõendab tulemust  

Kui lugeja saab aru, mida tehti, miks seda tehti ja näeb, et tulemus on olemas, siis on dokumentatsioon korrektne.
