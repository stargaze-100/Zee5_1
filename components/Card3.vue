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
                  > <!--class="fill-height flex-column"-->
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
          
          img: 'https://nettv4u.com/imagine/10-07-2020/kailasapuram.jpg',
        },
        {
          
          img: 'https://i.ytimg.com/vi/zhavQiEIvUc/maxresdefault.jpg',
        },
        {
          
          img: 'https://f7b4p3f8.stackpathcdn.com/wp-content/uploads/2020/09/confirm-of-a-huge-deal-for-ore-bujjiga.jpg',
        },
        {
          
          img: 'https://upload.wikimedia.org/wikipedia/en/1/1c/Kaafir_ZEE5_poster.jpg',
        },
        {
          
          img: 'https://s3images.zee5.com/wp-content/uploads/sites/48/2020/04/AmruthaRamam-poster-1.jpg',
        },
        {
          
          img: 'https://www.iwmbuzz.com/wp-content/uploads/2020/04/review-of-zee5s-bamfaad-brings-homethe-big-screen-experience-1280x720.jpeg',
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