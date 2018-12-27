<template lang='pug'>
#ffiotSlideshow
  .eg-slideshow
    slide
      center
        img(src='./logo.png' width='50%')
        h4 Was ist das?
        h4 Wie geht das?
        p adnidor, @hibas123, @margau_me

    slide(enter='fadeIn' leave='fadeOut')
      center
      h3 Motivation
      h4.
        "Ich bin der Meinung, wir brauchen mehr interne Dienste"
      p adnidor, irgendwann im Sommer beim FFS
      h4 Wie kann Freifunk mehr sein, als "nur" Transit?

    slide(enter='fadeIn' leave='fadeOut')
      h3 Idee
      h4.
        Wie wäre es, das Freifunk-Netz für selbstgebaute Sensoren zu nutzen?

    slide(enter='fadeIn' leave='fadeOut')
      h3 Konzept
      p.
        Wir wollen eine offene Plattform schaffen, mit der jeder leicht in die IoT-Welt - insbesondere für Sensoren - einsteigen kann.
      p.
        Dazu gehört sowohl Hardware mit Anleitungen, Workshops etc., als auch das Backend, welches Daten sammelt und bereitstellt.

    slide(enter='fadeIn' leave='fadeOut')
      h3 Konzept
      center
        h4 Mehr Details:
        p https://github.com/Freifunk-IoT/freifunk-iot-concept
        img(src='./github.png')

    slide(enter='fadeIn' leave='fadeOut')
      h2 Das 'S' in IoT steht für Security

    slide(enter='fadeIn' leave='fadeOut')
      h3 Projektumfang
      h4 Hardware
      ul
        li ESP8266/ESP32
        li Bosch XDK
        li Raspberry PI
        li ...

    slide(enter='fadeIn' leave='fadeOut')
      h3 Projektumfang
      h4 Backend
      ul
        li "Data Sink"
        li "Data Access" (APIs/Schnittstellen)
        li Authentication
        li Federation

    slide(enter='fadeIn' leave='fadeOut')
      h3 Projektumfang
      h4 Dokumentation
      ul
        li Tutorials
        li Hard- und Softwareexamples
        li PCB's
        li Workshops

    slide(enter='fadeIn' leave='fadeOut')
      h2 Demo

    slide(enter='fadeIn' leave='fadeOut')
      h3 Backend
      p.
        Fabian, du bist dran!

    slide(enter='fadeIn' leave='fadeOut')
      h3 Hardware
      ul
        li Zum selberbauen
        li verschiedene Boards
        li ESP-basiert

    slide(enter='fadeIn' leave='fadeOut')
      h3 Hardware
      h4 Sensoren
      ul
        li Temperatur
        li Luftfeuchtigkeit
        li Luftdruck
        li Licht
        li Schallpegel

    slide(enter='fadeIn' leave='fadeOut')
      h3 Hardware
      h4 Microcontroller
      ul
        li ESP8266
        li ESP32
        li Raspberry Pi

    slide(enter='fadeIn' leave='fadeOut')
      h3 Ausblick
      ul
        li Mehr Hardware
        li Workshops
        li Integration ins TTN
        li Federation
        li Ausbau des Backends

    slide(enter='fadeIn' leave='fadeOut')
      h2 Wer sind wir?
      ul
        li margau: @margau on Twitter (DECT: ????)
        li Hibas123: @hibas123 on Twitter (DECT: ????)
        li adnidor: @adnidor@chaos.social on Mastodon (DECT: 3677)

    slide(enter='fadeIn' leave='fadeOut')
      h2 Mitmachen
      ul
        li github.com/freifunk-iot
        li freifunk-iot@lists.freifunk-stuttgart.de
        li www.freifunk-iot.de

    slide(enter='fadeIn' leave='fadeOut')
      h2 Vielen Dank für eure Aufmerksamkeit!
      h3 Besucht uns an unserem Projekttisch!
</template>

<script>
import eagle from 'eagle.js'
export default {
  mixins: [eagle.slideshow],
  infos: {
    // These infos appear on the home page, below the slideshow's thumbnail
    title: 'Freifunk-IoT Vorstellung',
    description: 'Projektvorstellung & aktueller Stand (Deutsch)',
    path: 'ffiot-de'
  }
}
</script>

<style lang='scss'>
@import url(https://fonts.googleapis.com/css?family=Raleway);
#ffiotSlideshow {
    .eg-slideshow {
        font-family: 'Montserrat', sans-serif;
        background-color: #eef;
        .eg-slide {
            .eg-slide-content {
                width: 25em;
                max-width: 80%;
                margin: 0 auto;
            }
        }
    }
    .eg-slide-content {
        width: 25em;
        max-width: 80%;
        margin: 0 auto;
    }
}
</style>
