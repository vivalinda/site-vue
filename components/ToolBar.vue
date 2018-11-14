<template>
  <v-toolbar class="blue-grey darken-3">
    <VSpacer />
    <img 
      class="logoToolbar"
      src="@/static/logo.png" 
      alt="VIVALINDA" >
    <VSpacer />
  </v-toolbar>    
</template>

<script>
export default {
  data() {
    return {
      title: 'Vivalinda'
    }
  }
}
</script>

<style lang="stylus">
  .logoToolbar
    max-height 85%
</style>
