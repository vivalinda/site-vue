<template>
  <v-layout
    column
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <v-container
        grid-list-md
        class="blue-grey lighten-4"
        fluid 
      >
        <v-layout 
          row 
          wrap
          fluid
        >           <!-- The v-for in PhotoCard is starting in 1 ( num ) but the index 0 to ( num - 1) -->
          <PhotoCard   
            v-for="num in 6"
            :key="num-1"
            :photourl= "photoLocation(num)" 
          />
        </v-layout>
      </v-container>
    </v-flex>
  </v-layout>
</template>

<script>
import PhotoCard from '../components/PhotoCard.vue'

export default {
  components: {
    PhotoCard
  },
  data() {
    return {
      photo: this.photoLocation(2)
    }
  },
  methods: {
    photoLocation(num) {
      let stringNum = num.toString()
      return require(`../assets/img/photos/photo${num}.jpg`)
    }
  }
}
</script>
