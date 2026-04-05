---
layout: default
title: Mida tehti
nav_order: 3
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

## Näide (hea)

{: .green }
Näide (hea): paigaldati MariaDB andmebaasiserver käsuga `sudo apt install mariadb-server`, et teha tabeli loomise, varundamise ja taastamise etapid ühes keskkonnas.
(pilditõestus)

Kui tegu on tavapäraste üksteisele järgnevate käskudega ja tulemus on üks, võib kirjelduse kirjutada pikema lõiguna, kuid käsud tuleb siiski eraldi koodilõiguna välja tuua.

Näide 2 (hea): loodi andmebaas ja tabel, lisati näidisandmed, tehti varukoopia ning taastati andmed pärast tabeli kustutamist.

```bash
sudo apt update
sudo apt upgrade -y
sudo apt install mariadb-server -y
sudo systemctl enable mariadb
sudo systemctl start mariadb
mysql -u root -e "CREATE DATABASE projekt_db;"
mysqldump -u root projekt_db > projekt_db_dump.sql
mysql -u root -e "DROP TABLE projekt_db.customers;"
mysql -u root projekt_db < projekt_db_dump.sql
```

(Pilditõestus varundamisest ja taastamisest)

## Näide (halb)

Väldi:

- liiga üldisi lauseid nagu "tehti vajalikud muudatused"
- põhjendusi ja seletusi, miks midagi tehti
- loetelu, mis ei ütle, mida päriselt muudeti
- liiga detailset tööprotsessi, mis loetleb iga väikese sammu eraldi

{: .warning }
Näide (halb): seadistati server, tehti vajalikud muudatused ja pandi projekt käima
