<template>
  <v-carousel 
    cols="12" md="5"
    cycle
    hide-delimiter-background
    delimiter-icon="mdi-minus"
    show-arrows-on-hover
    class="pa-"
    align="center"
    justify="center"
  >
    <v-carousel-item
    cols="12" md="5"
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      width="1000"
      height="1600"
      centered
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          
          {
            src: 'https://www.dekhnews.com/entertainment/wp-content/uploads/2019/10/maxresdefault-35.jpg',
          },
          {
            src: 'https://cdn.dnaindia.com/sites/default/files/styles/full/public/2018/08/09/715886-lockdown-poster.jpg',
          },
          {
            src: 'https://i.ytimg.com/vi/bDfGQ00hsSU/maxresdefault.jpg',
          },
        ],
      }
    },
  }
</script>