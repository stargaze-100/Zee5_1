<template>
<v-responsive>
  <v-content class="purple darken-4" centered cols="16" xs="6" sm="10" md="14">
    <v-row no-gutters>
      <v-col cols="12" sm="4" pa="2" pl="4">
        
          <v-app-bar-nav-icon>
        <v-img class="ml-sm-16 mt-sm-10" src="https://upload.wikimedia.org/wikipedia/en/thumb/3/30/Zee5_Official_logo.svg/1200px-Zee5_Official_logo.svg.png" 
          width="60" height="60">
          </v-img>
        </v-app-bar-nav-icon>
        
      </v-col>
    
      <v-col cols="12" md="4" mx="4">
        
          <searchbar/>
         </v-col>

       <v-col :cols="12" xs="6" sm="3" >
        <v-card
          class="pa-2 mt-xs-n3 ml-md-14"
          outlined
          tile
          centered
          color="purple darken-4"
        >
           <v-btn class="rounded-circle ma-2">
            <v-icon>mdi-pencil</v-icon>
          </v-btn>

           <v-btn class="rounded-circle ma-2">
            <v-icon>mdi-wrench</v-icon>
          </v-btn>
          
          <v-btn class="rounded-circle ma-2">
            <v-icon>mdi-account</v-icon>
          </v-btn>
          
          <v-btn class="rounded-circle ma-2">
          <v-app-bar-nav-icon></v-app-bar-nav-icon>
          </v-btn>

          </v-card>
        </v-col>
      </v-row>

      <v-row>
         
        <v-col cols="12" xs="4" md="12">
          <v-card color="purple darken-4">
          <Shiftnav/>
          </v-card>
        </v-col>
      </v-row>
      
      <v-row>
        <v-col cols="12" xs="10">
              <v-card color="purple darken-4"
              align="center"
              justify="center">
                <Slide1/>
              </v-card>

            </v-col>
            </v-row>
        
        <v-card 
          color="black"
          class="mt-sm-5"
          height="1500">
            <v-carousel hide-delimiters>
            <v-card
            align ="left"
            justify="left"
            class="pl-16 ml-16 ma-2 mr-n16 black">
            <div class="col-2 ml-16 pl-16 text-truncate black">
              <h1>Top shows</h1>
            </div>
            </v-card>

              <v-carousel-item>
                <Cards/>
              </v-carousel-item>
              <v-carousel-item>
                <Card2/>
              </v-carousel-item>
            </v-carousel>
            
              <v-carousel hide-delimiters>
              <v-carousel-item>
                <Card4/>
              </v-carousel-item>
              <v-carousel-item>
                <Card3/>
              </v-carousel-item>
            </v-carousel>
            </v-card>
        
    </v-content>
  </v-responsive>
</template>

<script>

</script>