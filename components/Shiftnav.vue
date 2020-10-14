<template
color="black">
  <v-bottom-navigation
    class="md-6 sm-4 mb-n6"
    v-model="bottomNav"
    dark
    shift
    color="pink"
  >
    <Filter0/>
    <v-btn>
      <span>Home</span>
      <v-icon>mdi-home</v-icon>
    </v-btn>

    <v-btn>
      <span>Originals</span>
      <v-icon>mdi-television-play</v-icon>
    </v-btn>

    <v-btn>
      <span>Club</span>
      <v-icon>mdi-book</v-icon>
    </v-btn>

    
    <v-btn>
      <span>More</span>
      <v-icon>mdi-apps</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>

<script>
  export default {
    data () {
      return {
        bottomNav: 3,
      }
    },

    computed: {
      color () {
        switch (this.bottomNav) {
          case 0: return 'blue-grey'
          case 1: return 'teal'
          case 2: return 'brown'
          case 3: return 'indigo'
        }
      },
    },
  }
</script>