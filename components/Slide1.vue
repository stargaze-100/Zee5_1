<template>
  <v-carousel 
    style="background-color:#2B1031"
    cycle
    hide-delimiter-background
    delimiter-icon="mdi-minus" 
    show-arrows-on-hover
    class=""
    align="center"
    justify="center"
  > <!--minus sign from the high fidelity prototype-->
    <v-carousel-item
    cols="12" md="5" sm="6" xs="12"
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      
      width="1000"
      
      centered
    ><!--Featured series of zee5-->
    </v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        items: [
           {
            src: 'https://i.ytimg.com/vi/bDfGQ00hsSU/maxresdefault.jpg',
          },
          {
            src: 'https://www.dekhnews.com/entertainment/wp-content/uploads/2019/10/maxresdefault-35.jpg',
          },
          {
            src: 'https://cdn.dnaindia.com/sites/default/files/styles/full/public/2018/08/09/715886-lockdown-poster.jpg',
          },
          {
            src: 'https://m.media-amazon.com/images/M/MV5BZmI1Y2YzMDctNDI3NC00YmRjLTk4NjYtOWVjMDQxNWE0MDBkXkEyXkFqcGdeQXVyMjUxMTY3ODM@._V1_.jpg',
          },
          {
            src: 'https://akamaividz2.zee5.com/image/upload/w_1170,h_658,c_scale,f_auto,q_auto/resources/0-1-337909/list/1170x658withlog_1175111418.jpg',
          },
          {
            src: 'https://www.news23.in/wp-content/uploads/2020/09/poison-2-on-zee5-release-date-cast-trailer.jpg',
          },
        ],
      }
    },
  }
</script>