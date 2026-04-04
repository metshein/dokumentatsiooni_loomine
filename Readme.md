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

👉 Täpsem juhend: [Dokumentatsiooni juhend](https://github.com/metshein/dokumentatsiooni_loomine/wiki)

## Pikk versioon

Dokumentatsiooni eesmärk sõltub kontekstist, kuid põhimõte on sama – tehtud töö peab olema arusaadav, põhjendatud ja kasutatav ka teiste poolt.
Õppetöös on dokumentatsioon tehniline tõendusmaterjal. Selle abil näidatakse, mida tehti, miks seda tehti ja kas autor saab tehtud tööst aru.

Päriselus on dokumentatsiooni roll praktilisem:
- süsteemi saaks üles ehitada ja taastada  
- teised saaksid aru, kuidas see töötab  
- haldus ja veaotsing oleks võimalik  

Hea dokumentatsioon ühendab need mõlemad. See ei kirjelda ainult tegevusi, vaid selgitab otsuseid ja tõendab tulemust nii, et teine inimene saab aru, mis tehti, miks seda tehti ja kuidas sama lahendus uuesti toimima panna.

## 1. Mida tehti

Kirjelda konkreetselt tehtud tegevused. Väldi üldsõnalisi lauseid:
- "seadistati süsteem"
- "tehti vajalikud muudatused"

Too välja:
- milline tegevus tehti  
- millise käsu või tööriistaga  

Näide (halb):
- seadistati server

Näide (hea):
- paigaldati tarkvara käsuga `sudo apt install pakett`

---

## 2. Miks tehti

Iga oluline tegevus peab olema põhjendatud.

Näita:
- miks see samm oli vajalik  
- mida see lahendab või võimaldab  

Näide (halb):
- muudeti seadistust

Näide (hea):
- seadistust muudeti, et piirata ligipääsu ainult lokaalsele masinale

---

## 3. Milline on tulemus

Dokumentatsioon peab näitama lõpptulemust ja selle kontrolli.

Too välja:
- kuidas kontrolliti  
- milline oli tulemus  

Näide (halb):
- süsteem töötab

Näide (hea):
- kontrolliti teenuse olekut käsuga `systemctl status teenus`  
- tulemuseks oli `active (running)`, mis kinnitab, et teenus töötab  

Tõestus võib olla:
- käsu väljund (kopeeritud tekst)  
- logi või päringu tulemus  
- ekraanipilt  
- link (kui viib otsesele ja kontrollitavale tulemusele)  

Oluline:
- tõestus peab olema kontrollitav  
- tõestus peab olema seotud väitega (ei tohi olla suvaline pilt või väljund)  

---

## 4. Tõestus

Iga oluline tulemus peab olema tõendatav.

Sobivad tõestused:
- käsu väljund  
- logi või päringu tulemus  
- ekraanipilt  
- link (kui see viib otsesele tulemusele)

Näide:
- teenuse olek kontrolliti käsuga `systemctl status teenus`  
- väljund näitas `active (running)`

---

## 5. Vormistus ja kirjutamisviis

Dokumentatsioon kirjutatakse umbisikulises vormis.

Kasutatakse:
- tehti, paigaldati, muudeti  

Ei kasutata:
- ma tegin, paigaldasin, muutsin  

Näide (halb):
- paigaldasin tarkvara ja muutsin faili

Näide (hea):
- tarkvara paigaldati ja konfiguratsioonifaili muudeti  

Käsud ja kood esitatakse:
- lühikesed käsud teksti sees (`käsk`)  
- pikemad käsud eraldi plokis (taandega)

Näide:
- `sudo apt install pakett`

Kui dokumentatsioon kirjutatakse tekstiredaktoris (nt Drive Document), siis:
- koodi ja käske kuvatakse monoruumi fondiga (nt **Courier New**, **Consolas**)  

See aitab eristada käske ja muud teksti ning muudab dokumentatsiooni loetavamaks.

---

## 6. Soovituslikud tööriistad dokumentatsiooni tegemiseks

Dokumentatsiooni saab teha erinevate tööriistadega, sõltuvalt eesmärgist. Järgi juhendaja soovitusi.

**Lihtne ja levinud:**
- Microsoft Word – aruanded ja esitatavad tööd. Jaga pilvekeskkonnas (Google Drive, OneDrive jms)  
- Google Docs – koostöö ja jagamine  

**Tehniline dokumentatsioon:**
- Markdown (.md) – README failid ja projektid GitHubis  
- Visual Studio Code – Markdown kirjutamine koos eelvaatega  
- Typora – kirjutamine koos kohese visuaalse eelvaatega  
- Obsidian – suuremad ja omavahel seotud dokumentatsioonid  

**Projektipõhine dokumentatsioon:**
- GitHub Wiki – mitmelehelised juhendid ja projektidokumentatsioon  

Oluline ei ole tööriist, vaid see, et dokumentatsioon oleks:
- arusaadav  
- põhjendatud  
- kontrollitav
