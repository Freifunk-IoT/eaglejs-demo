<template lang='pug'>
#ffiotSlideshow
  .eg-slideshow
    slide
      h1 Freifunk-IoT
      h4 Was ist das?
      h4 Wie geht das?
      p @adnidor, @hibas123, @margau_me

    slide(enter='bounceInRight' leave='fadeOut')
      h3 Hey modify me !
      p.
        Come on modify me ! If you are running the development server,
        you will see the changes take effect immediately

    slide(enter='fadeIn')
      h3 Want cool effects?
      p.
        Code your own, or try stealing for the other slideshows !
</template>

<script>
import eagle from 'eagle.js'
export default {
  mixins: [ eagle.slideshow ],
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
#ffiotSlideshow{
  .eg-slideshow{
    font-family: 'Raleway';
    background-color: #eef;
    .eg-slide{
      .eg-slide-content{
        width: 25em;
        max-width: 80%;
        margin: 0 auto;
      }
    }
  }
  .eg-slide-content{
    width: 25em;
    max-width: 80%;
    margin: 0 auto;
  }
}
</style>
