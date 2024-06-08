# Radion Kanavat

Suomessa on käytössä kaksi virallista kanavaa:

- **LongFast**: Salausavain on `AG==`, ja sen pitäisi olla oletuksena.
- **Radio**: Ei ole salausavainta, eli poista avain, jonka sovellus luo.

On olemassa myös `admin`-kanava, jolla voi etänä muokata omien radioiden asetuksia, jos on radioetäisyydellä. Kanavan salausavainta **EI SAA MISSÄÄN NIMESSÄ JAKAA!**

## Kanavan Luominen

1. Mene radion asetuksiin ja etsi kohta, jossa lukee `channels`. Paina siitä.

   <img src="../assets/kanavat/3_dots.jpg" width="300"/>
   <img src="../assets/kanavat/configuration.jpg" width="300"/>
   <img src="../assets/kanavat/channels.jpg" width="200"/>

2. Kanavat ladataan radiosta. Riippuen yhteyden laadusta ja kanavien määrästä, tämä voi kestää hetken.

   <img src="../assets/kanavat/loading channels.jpg" width="200"/>

3. Kun kanavat-sivu on auennut, voit luoda uuden kanavan painamalla vihreää plussaa. LongFast on oletuksena, joten sitä ei tarvitse luoda.

4. Sijainnin tarkkuuden voi asettaa omien mieltymysten mukaan.

5. LongFastissa ei tarvitse laittaa uplink ja downlink päälle, sitä käytetään MQTT-verkossa, jota tässä ohjeessa ei käytetä.

6. Radio-kanavaan **EI SAA LAITTAA** uplink ja downlink päälle!

   <img src="../assets/kanavat/create channel.jpg" width="200"/>
   <img src="../assets/kanavat/LongFast.jpg" width="200"/>
   <img src="../assets/kanavat/Radio.jpg" width="200"/>

7. Kun olet valmis, paina `Save`, jotta kanava lisätään listaan. Lopuksi paina vihreää `Send`-nappia, niin kanavat lähetetään radiolle.

   <img src="../assets/kanavat/send_channels.jpg" width="250"/>

8. Näyttöön aukeaa pieni ikkuna, joka näyttää lähetyksen edistymisen. Kun palkki häviää, voit sulkea asetukset.

   <img src="../assets/kanavat/sending_channels.jpg" width="200"/>
   <img src="../assets/kanavat/channels_sent.jpg" width="200"/>

Jos näet kanavat näin, onnittelut! Onnistuit luomaan kanavan/kanavat.

<img src="../assets/kanavat/channels_home.jpg" width="250"/>

---
