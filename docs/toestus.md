---
layout: default
title: Tõestus
nav_order: 6
---

# Tõestus

Selles peatükis esitad kontrollitavad tõendid, mis kinnitavad eelmises peatükis toodud tulemusi.

Lihtne reegel: iga tulemuse väite juurde lisa vähemalt üks kontrollitav tõend.

Sobivad tõestused:

- käsu väljund (kopeeritud tekst)
- logi või päringu tulemus
- ekraanipilt
- link, kui see viib otseselt kontrollitava tulemuseni

## Oluline

- tõestus peab olema kontrollitav
- tõestus peab olema seotud väitega
- tõestus peab olema loetav (ära lisa liiga pikka toorväljastust ilma selgituseta)

## Näide

- Väide: MariaDB teenus töötab
- Tõestus: käsu `systemctl status mariadb` väljundis on seisund `active (running)`
- Väide: tabel `customers` on loodud
- Tõestus: päringu `SHOW TABLES;` tulemustes on näha `customers`
- Väide: andmed taastati varukoopiast
- Tõestus: taastamise järel `SELECT * FROM customers;` kuvab enne kustutamist sisestatud read
