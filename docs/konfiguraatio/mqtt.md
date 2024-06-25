# MQTT:n käyttöönotto Meshtasticissa: Lyhyt opas (Ilman CLI:tä)

Meshtastic on monipuolinen ja avoimen lähdekoodin viestintäalusta, jota voidaan parantaa MQTT:llä (Message Queuing Telemetry Transport) laajempia viestintäominaisuuksia varten. Tässä on nopea opas MQTT:n käyttöönottoon Meshtastic-laitteillesi.

## Edellytykset

1. **Meshtastic-laite**: Varmista, että laitteesi on oikein asennettu ja toimii.
2. **Meshtasticin laiteohjelmisto**: Päivitä laitteesi uusimpaan laiteohjelmistoversioon, joka tukee MQTT:tä.
3. **MQTT-välityspalvelin**: Käytä oletus-MQTT-välityspalvelinta `mqtt.meshtastic.org` tai asenna oma välityspalvelin, jos haluat.

## Vaiheittainen opas

### 1. Pääsy laitteen asetuksiin

1. **Odota laitteen käynnistymistä ja yhdistymistä**: Odota, että Meshtastic-laite käynnistyy ja yhdistyy.
2. **Avaa asetukset**: Siirry Meshtastic-sovelluksen tai verkkokäyttöliittymän asetuksiin tai kokoonpanokohtaan.

### 2. MQTT-asetusten määrittäminen

1. **Etsi MQTT-asetukset**: Löydä MQTT-asetusten konfigurointikohta asetusten valikosta.
2. **Ota MQTT käyttöön**: Ota MQTT käyttöön kytkemällä asetusta.
3. **Aseta MQTT-välityspalvelin**: Jos ei ole jo asetettu, anna oletus MQTT-välityspalvelimen osoite ja portti.
   - **Välityspalvelimen osoite**: `mqtt.meshtastic.org`
   - **Portti**: `1883` (oletusportti)
4. **Aseta MQTT-juuriaihe**: Anna juuriaiheeksi `msh/Finland`.
5. **Tallenna muutokset**: Paina `Lähetä`-painiketta tallentaaksesi MQTT-asetukset. Laite käynnistyy uudelleen automaattisesti.

### 3. Ylälähetyksen ja alalähetyksen ottaminen käyttöön tietyillä kanavilla

1. **Odota laitteen käynnistymistä ja yhdistymistä**: Odota, että Meshtastic-laite käynnistyy ja yhdistyy uudelleen MQTT-asetusten tallentamisen jälkeen.
2. **Etsi kanava-asetukset**: Siirry kanavien konfigurointikohtaan.
3. **Valitse kanava (LongFast)**: Valitse `LongFast`-kanava (tai muut haluamasi kanavat).
4. **Ota ylälähetys käyttöön**: Ota ylälähetys käyttöön kytkemällä asetusta valitulla kanavalla.
5. **Ota alalähetys käyttöön**: Ota alalähetys käyttöön kytkemällä asetusta valitulla kanavalla.
6. **Tallenna muutokset**: Paina `Lähetä`-painiketta tallentaaksesi kanava-asetukset. Laite käynnistyy uudelleen automaattisesti.

### 4. MQTT:n sivuuttamisen poistaminen käytöstä LoRa-asetuksissa

1. **Odota laitteen käynnistymistä ja yhdistymistä**: Odota, että Meshtastic-laite käynnistyy ja yhdistyy uudelleen kanava-asetusten tallentamisen jälkeen.
2. **Etsi LoRa-asetukset**: Siirry LoRa-asetusten kohtaan.
3. **Poista `Ignore MQTT` käytöstä**: Varmista, että `Ignore MQTT`-asetus on poistettu käytöstä.
4. **Tallenna muutokset**: Paina `Lähetä`-painiketta tallentaaksesi LoRa-asetukset. Laite käynnistyy uudelleen automaattisesti.

### 5. Konfiguraation vahvistaminen

1. **Odota laitteen käynnistymistä ja yhdistymistä**: Odota, että Meshtastic-laite käynnistyy ja yhdistyy uudelleen LoRa-asetusten tallentamisen jälkeen.
2. **Vahvista asetukset**: Tarkista asetukset uudelleen varmistaaksesi, että MQTT-konfiguraatio on aktiivinen ja kaikki muutokset on sovellettu.

## Yhteenveto

Noudattamalla näitä ohjeita saat MQTT:n onnistuneesti käyttöön Meshtastic-laitteellasi käyttäen juuriaihetta `msh/Finland`. Varmista, että vain halutuilla kanavilla on ylälähetys ja alalähetys käytössä ja että LoRa-asetusten `Ignore MQTT` -asetus on poistettu käytöstä. Muista, että laite käynnistyy automaattisesti uudelleen aina, kun painat `Lähetä`-painiketta asetusten muuttamisen jälkeen. Nauti parannetuista viestintäominaisuuksista Meshtastic-verkossasi!
