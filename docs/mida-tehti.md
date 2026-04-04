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

> Näide (hea): paigaldati PostgreSQL andmebaasiserver, et rakendus saaks andmeid püsivalt salvestada ja päringuid teha.
>
> Koodinäide:
>
> ```bash
> sudo apt install postgresql
> sudo systemctl enable postgresql
> sudo systemctl start postgresql
> sudo -u postgres psql -c "CREATE DATABASE projekt_db;"
> ```
>
> (Pilditõestus andmebaasi loomisest)
> {: .green }

Väldi:

- liiga üldisi lauseid nagu "tehti vajalikud muudatused"
- põhjendusi ja seletusi, miks midagi tehti
- loetelu, mis ei ütle, mida päriselt muudeti
- liiga detailset tööprotsessi, mis loetleb iga väikese sammu eraldi

{: .warning }
Näide (halb): seadistati server, tehti vajalikud muudatused ja pandi projekt käima
