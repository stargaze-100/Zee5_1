<template>
  <v-container class="pa-4">
    <v-row align="center" justify="center">
      <template v-for="(item, i) in items">

        <v-col
          :key="i"
          cols="6"
          md="4"
          sm="4"
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
          
          img: 'https://i2.wp.com/theyellowdaal.com/wp-content/uploads/2020/08/images-4.jpeg?fit=690%2C390',
        },
        {
          
          img: 'https://s3images.zee5.com/wp-content/uploads/sites/48/2020/06/Mafia.jpg',
        },
        {
          
          img: 'https://akamaividz2.zee5.com/image/upload/w_541,h_304,c_scale,f_auto,q_auto/resources/0-1-389062/list/1170x658withlogo_963494813.jpg',
        },
        {
          
          img: 'https://i.ytimg.com/vi/yDpUASu9CYs/maxresdefault.jpg',
        },
        {
          
          img: 'https://www.mumbailive.com/images/media/images/images_1591981206516_WhatsApp_Image_2020_06_12_at_10.00.06_PM.jpeg?bg=471e1b&crop=1280%2C718.5964912280701%2C0%2C365.95778012767784&fit=crop&fitToScale=w%2C1368%2C768&h=606.3157894736842&height=1280&w=1080&width=1280',
        },
        {
          
          img: 'https://newsbust.in/wp-content/uploads/2020/05/With-HyperShorts-Games-and-News-2.0-ZEE5-wants-to-become.jpg',
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