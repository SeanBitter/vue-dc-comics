<template>
  <div id="app">
    <TheHeader/>
    <TheMain/>
    <BlueBanner/>
    <TheFooter/>
    <SignUpBanner/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import BlueBanner from './components/BlueBanner.vue'
import TheFooter from './components/TheFooter.vue'
import SignUpBanner from './components/SignUpBanner.vue'
import TheMain from './components/TheMain.vue'

export default {
  name: 'App',
  components: {
    TheHeader,
    BlueBanner,
    TheFooter,
    SignUpBanner,
    TheMain,
  }
}
</script>

<style lang="scss">

@import "assets/scss/main.scss";

</style>
