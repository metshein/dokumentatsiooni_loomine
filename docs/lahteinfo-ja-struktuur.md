---
layout: default
title: Lähteinfo ja struktuur
nav_order: 2
---

# Lähteinfo ja struktuur

Esimesena lisa alati eesmärk, mida tegema hakkad. Kirjelda 2-4 lausega oma sõnadega, mida oli vaja saavutada, mis pidi tulemuseks valmima.

Näidis:

Töö eesmärk on kontrollitud olukorras läbi teha andmebaasi varundamise ja taastamise protsess MariaDB keskkonnas. Ülesande käigus luuakse andmebaas ja tabel, imporditakse näidisandmed, lisatakse üks isiklik kirje, tehakse loogiline ja füüsiline varukoopia, kustutatakse tabel ning taastatakse andmed füüsilisest varukoopiast.

## Õpetaja antud ülesanne

Kui õpetaja annab ülesande, kirjuta selle põhinõuded lühikese kokkuvõttena, mitte pika copy-paste tekstina.

## Keskkond ja masinad

Kui töö tehakse mitmes masinas, kirjelda iga masina roll, nimi ja võrguandmed eraldi. Nii saab juhendaja aru, kus teenused jooksevad ja kuidas masinad omavahel suhtlevad.

Too välja:

- masina nimi (hostname) ja roll, näiteks app-server või db-server
- masina IP-aadress ja vajadusel võrk
- IP-plaan (IP võrkude plaan ja IP aadresside plaan)
- operatsioonisüsteem ja versioon
- milline teenus jookseb millises masinas
- peamiste konfiguratsioonifailide asukohad

Näidis:

- vm-app, roll: rakenduse server, IP: 192.168.56.10, Ubuntu 22.04, teenus: Apache
- vm-db, roll: andmebaasi server, IP: 192.168.56.11, Ubuntu 22.04, teenus: MariaDB
- konfiguratsioonid: /etc/apache2/sites-available/app.conf ja /etc/mysql/mariadb.conf.d/50-server.cnf

## Põhimõisted (kutseeksam)

Kui kutseeksam nõuab põhimõistete loetelu, lisa see siia eraldi alajaotusse.

Kuidas mõisteid valida:

- vali mõisted, mida töös päriselt kasutasid
- vali mõisted, ilma milleta ei saa lugeja sinu samme ja tulemustest aru
- eelista mõisteid, mis seostuvad teenuste, võrgu, turbe ja seadistustega
- väldi üldsõnu, mis ei aita töö kontrollimisel

Kui palju selgitada:

- iga mõiste kohta 1 lühike definitsioon
- lisa 1 lühike lause, kuidas seda mõistet selles töös kasutati
- väldi pikka teooriat, eesmärk on praktiline arusaadavus
- soovituslik maht on 8-12 mõistet

Näidisvorm:

- MariaDB: relatsiooniline andmebaasihaldur. Selles töös kasutati seda rakenduse andmete salvestamiseks.
- Hostname: masina nimi võrgus. Selles töös eristati selle abil rakenduse ja andmebaasi serverit.
- Gateway: marsruuter, mille kaudu liiklus liigub teistesse võrkudesse. Selles töös määrati gateway võrguühenduse toimimiseks.

## Kontrolli eeldused juhendajale

Kirjelda, mida hindaja peab teadma enne kontrollimist. Reeglina dokumentatsiooni ei lisata päris paroole ja seepärast saa kinnitus juhendajalt, et kuidas paroolid edastatakse.
