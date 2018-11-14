<template>
  <v-app dark>
    <ToolBar />
    <v-content>
      <nuxt />
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import ToolBar from '@/components/ToolBar.vue'
import Footer from '@/components/Footer.vue'

export default {
  components: {
    ToolBar,
    Footer
  }
}
</script>
