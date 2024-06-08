# Laitteisto-opas aloittelijoille

- Oppaan tavoite:

  - esitellä rajallinen määrä laitteita
    - plussat ja miinukset
  - muita huomioita

- [Meshtastic-dokumentaatiosivuilla](https://meshtastic.org/docs/hardware/devices/) on hyvää teknistä tietoa tuetuista laitteista.

## Kuinka monta laitetta tarvitsen tai haluan alussa?

- 1 tai 2, riippuen siitä haluatko kokeilla ja tutustua teknologiaan

  - 1 laite mukaasi
  - 2. laite kotiin tai perheenjäsenelle
  - onko lähelläsi muita solmuja, joiden kanssa haluat viestiä

- 3+
  - ok, mutta älä innostu liikaa ennen kuin olet tutustunut, harkitse tarvitsemiasi ominaisuuksia

## Koteloita

- 3D-tulostus, valmiit, kirjasto, muovirasia, jäätelöpakkaus, alkuperäinen laatikko, kuvia?

## Paristot

- On erittäin tärkeää ymmärtää turvallisuus kaikentyyppisten paristojen käytössä
  - erityisesti litiumparistot
    - LIPOs
  - 18650
  - muut
- Saatat joutua ostamaan ja asentamaan oman pariston laitteeseen

## Antenni

- Varmista, että antenni on kytketty laitteeseen, kun se on päällä.

## Huomioitavat ominaisuudet

- Virrankulutus / tehokkuus
  - Mieti, miten aiot syöttää laitteeseen virtaa
    - USB-portti / laturi
  - USB-virtapankki
  - Oma paristo
- Taajuus
  - 868 MHz
  - 433 MHz käyttö on hyvin rajoitettua
- GPS
  - GPS-malli, antennin koko
  - Laite voi myös käyttää puhelimen paikannustietoja
- Näyttö
  - OLED
  - ePaper
  - ei näyttöä
- Prosessori
  - ESP32 vs ESP32s3 vs nRF52840
- GPIO

## Harkittavat laitteet

- Heltec

  - edullisempi
    - ellei ala miettimään paristokäyttöä tai aurinkovoimaa
  - melko virtaahaluava, erittäin tehottomasti käyttää paristoja (oma lipo ja virtapankki)
  - ok pöytäkäyttöön ja satunnaiseen kannettavaan käyttöön
  - laitteet tulevat yleensä paristoliittimen kanssa, joka täytyy liittää paristoon

- LilyGO

  - Tehokas virranhallinta
  - Hyvä kannettavaan radioon, joka toimii päivän tai enemmän ilman latausta
  - Mallet sisältävät tyypillisesti 18650-paristopidikkeen takana
    - asennettaessa paristoa, laita nauha sen ympärille, jotta se on helppo vetää ulos

- RAK
  - vähävirtainen
  - ihanteellinen aurinkovoimaan
  - langattomat laiteohjelmistopäivitykset
