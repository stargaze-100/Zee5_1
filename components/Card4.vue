<template>
  <v-container class="pa-4 text-center">
    <v-row align="center" justify="center">
      <template v-for="(item, i) in items">

        <v-col
          :key="i"
          cols="12"
          md="4"
        >
          <v-hover v-slot:default="{ hover }">
            <v-card
            
              :elevation="hover ? 12 : 2"
              :class="{ 'on-hover': hover }"
            >
              <v-img
                :src="item.img"
              ><!--Call the images from script-->
                <v-card-title>
                  <v-row
                   
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
          
          img: 'https://english.reportertodaynews.com/wp-content/uploads/2019/08/IMG-20190804-WA0040-750x430.jpg',
        },
        {
          
          img: 'https://i.ytimg.com/vi/GuONwXthPqE/hqdefault.jpg',
        },
        {
          
          img: 'https://moviespie.com/wp-content/uploads/2020/06/47-days-Telugu-Movie-to-Release-Directly-on-Zee5.jpg',
        },
        {
          
          img: 'https://www.grabon.in/indulge/wp-content/uploads/2020/04/Hotel-Mumbai.jpg',
        },
        {
          
          img: 'https://i.ytimg.com/vi/CQCDA0avvco/maxresdefault.jpg',
        },
        {
          
          img: 'https://akamaividz2.zee5.com/image/upload/w_1170,h_658,c_scale,f_auto,q_auto/resources/0-1-221079/list/water_bottel_mot_562341982.jpg',
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