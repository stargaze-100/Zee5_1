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
            
              :elevation="hover ? 12 : 2"
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
          
          img: 'https://www.letsott.com/assets/uploads/posts/Lockup.jpg',
        },
        {
          
          img: 'https://thenewscrunch.com/wp-content/uploads/2020/03/mentalhood-webseries-review.jpg',
        },
        {
          
          img: 'https://i.ytimg.com/vi/--9KtRec2js/hqdefault.jpg',
        },
        {
          
          img: 'https://flixoye.com/wp-content/uploads/2020/08/london-confidential-official-tea.jpg',
        },
        {
          
          img: 'https://i.ytimg.com/vi/PFskeOyEnO4/sddefault.jpg#404_is_fine',
        },
        {
          
          img: 'https://akamaividz2.zee5.com/image/upload/w_1170,h_658,c_scale,f_auto,q_auto/resources/0-1-276471/list/judgement_day_mo_630157257.jpg',
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
  opacity: 0.8;
 }


</style>