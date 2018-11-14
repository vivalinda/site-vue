<template>
  <v-flex
    xs12
    sm6 
    md4 
    lg4
    d-flex
  >
    <v-card class="vcard">
      <v-img  
        :src= "photourl"
        lazy-src="https://picsum.photos/10/6?image=77"
        aspect-ratio="1"
      >
        <v-layout
          slot="placeholder"
          fill-height
          align-center
          justify-center
          ma-0
        >
          <v-progress-circular 
            indeterminate 
            color="grey lighten-5"
          />
        </v-layout>
      </v-img>
    </v-card>
  </v-flex>
</template>

<script>
export default {
  props: {
    photourl: {
      type: String,
      default: require('../static/logo.png')
    }
  }
}
</script>
