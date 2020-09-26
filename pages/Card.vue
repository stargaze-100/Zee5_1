<template>
  <v-container class="pa-4 text-center">
    <v-row class="fill-height" align="center" justify="center">
      <template v-for="(item, i) in items">
        <v-col
          :key="i"
          cols="12"
          md="4"
        >
          <v-hover v-slot:default="{ hover }">
            <v-card
              :elevation="hover ? 14 : 2"
              :class="{ 'on-hover': hover }"
            >
              <v-img
                :src="item.img"
                height="225px"
              >
                <v-card-title>
                  <v-row
                    class="fill-height flex-column"
                    justify="space-between"
                  >
                  </v-row>
                </v-card-title>
              </v-img>
            </v-card>
          </v-hover>
        </v-col>
      </template>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      
      items: [
        {
          
          img: 'https://i2.wp.com/theyellowdaal.com/wp-content/uploads/2020/08/images-4.jpeg?fit=690%2C390',
        },
        {
          
          img: 'https://s3images.zee5.com/wp-content/uploads/sites/48/2020/06/Mafia.jpg',
        },
        {
          
          img: 'https://akamaividz2.zee5.com/image/upload/w_541,h_304,c_scale,f_auto,q_auto/resources/0-1-389062/list/1170x658withlogo_963494813.jpg',
        },
      ],
      transparent: 'rgba(255, 255, 255, 0)',
    }),
  }
</script>

<style scoped>
.v-card {
  transition: opacity .4s ease-in-out;
}

.v-card:not(.on-hover) {
  opacity: 0.6;
 }


</style>