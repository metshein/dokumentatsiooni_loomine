---
layout: default
title: Mida tehti
nav_order: 2
---

# Mida tehti

Kirjelda konkreetselt, mis tegelikult ära tehti. Siia käib töö tegevuste kujul, mitte üldine jutt. Kirjuta nii, et lugeja saab aru, millised sammud projekti jooksul tehti ja mida oleks võimalik vajadusel uuesti teha.

Tavaline tegevus projektides on näiteks:

- keskkonna ettevalmistamine
- tarkvara paigaldamine
- seadistuse muutmine
- failide või konfiguratsiooni lisamine
- teenuse käivitamine ja kontrollimine
- testi või kontrollsamme läbiviimine

Kirjelda tegevusplokke, mitte iga üksikut hiireklõpsu või klahvivajutust. Kui sama tüüpi tegevust tehti mitu korda, piisab ühest selgest kirjeldusega näitest või lühikesest kokkuvõttest.

Hea reegel on see: kui tegevuse saab hiljem sama järgi uuesti teha, siis see kuulub siia.

{: .green }
Näide (hea): paigaldati PostgreSQL andmebaasiserver käsuga `sudo apt install postgresql`, et rakendus saaks andmeid püsivalt salvestada.
(pilditõestus)

Kui tegu on tavapäraste üksteisele järgnevate käskudega ja tulemus on üks, võib kirjelduse kirjutada pikema lõiguna, kuid käsud tuleb siiski eraldi koodilõiguna välja tuua.

Näide 2 (hea): uuendati paketiloendeid, paigaldati PostgreSQL ning loodi rakenduse jaoks andmebaas.

```bash
sudo apt update
sudo apt upgrade -y
sudo apt install postgresql postgresql-contrib -y
sudo systemctl enable postgresql
sudo systemctl start postgresql
sudo -u postgres psql -c "CREATE DATABASE projekt_db;"
```

(Pilditõestus andmebaasi loomisest)

Väldi:

- liiga üldisi lauseid nagu "tehti vajalikud muudatused"
- põhjendusi ja seletusi, miks midagi tehti
- loetelu, mis ei ütle, mida päriselt muudeti
- liiga detailset tööprotsessi, mis loetleb iga väikese sammu eraldi

{: .warning }
Näide (halb): seadistati server, tehti vajalikud muudatused ja pandi projekt käima
