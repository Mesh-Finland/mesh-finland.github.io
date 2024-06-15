# Radion Kanavat

Suomessa on käytössä kaksi virallista kanavaa:

- **LongFast**: Salausavain on `AQ==`, ja sen pitäisi olla oletuksena.
- **Radio**: Ei ole salausavainta, eli poista avain, jonka sovellus luo.

On olemassa myös `admin`-kanava, jolla voi etänä muokata omien radioiden asetuksia, jos on radioetäisyydellä. Kanavan salausavainta **EI SAA MISSÄÄN NIMESSÄ JAKAA!**

## Kanavan Luominen

1. Mene radion asetuksiin ja etsi kohta, jossa lukee `channels`. Paina siitä.

   ![image](../assets/kanavat/3_dots.jpg ":size=25%")
   ![image](../assets/kanavat/configuration.jpg ":size=25%")
   ![image](../assets/kanavat/channels.jpg ":size=25%")

2. Kanavat ladataan radiosta. Riippuen yhteyden laadusta ja kanavien määrästä, tämä voi kestää hetken.

   ![image](../assets/kanavat/loading_channels.jpg ":size=25%")

3. Kun kanavat-sivu on auennut, voit luoda uuden kanavan painamalla vihreää plussaa. LongFast on oletuksena, joten sitä ei tarvitse luoda.

4. Sijainnin tarkkuuden voi asettaa omien mieltymysten mukaan.

5. LongFastissa ei tarvitse laittaa uplink ja downlink päälle, sitä käytetään MQTT-verkossa, jota tässä ohjeessa ei käytetä.

6. Radio-kanavaan **EI SAA LAITTAA** uplink ja downlink päälle!

   ![image](../assets/kanavat/create_channel.jpg ":size=25%")
   ![image](../assets/kanavat/LongFast.jpg ":size=25%")
   ![image](../assets/kanavat/Radio.jpg ":size=25%")

7. Kun olet valmis, paina `Save`, jotta kanava lisätään listaan. Lopuksi paina vihreää `Send`-nappia, niin kanavat lähetetään radiolle.

   ![image](../assets/kanavat/send_channels.jpg ":size=25%")

8. Näyttöön aukeaa pieni ikkuna, joka näyttää lähetyksen edistymisen. Kun palkki häviää, voit sulkea asetukset.

   ![image](../assets/kanavat/sending_channels.jpg ":size=25%")
   ![image](../assets/kanavat/channels_sent.jpg ":size=25%")

Jos näet kanavat näin, onnittelut! Onnistuit luomaan kanavan/kanavat.

![image](../assets/kanavat/channels_home.jpg ":size=25%")
