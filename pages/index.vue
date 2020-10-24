<template>
<v-responsive>
  <v-content class="purple darken-4" centered>
    <v-row no-gutters>
      <v-col cols="2" sm="2" md="3"> 
        
          <v-app-bar-nav-icon>
        <v-img aspect-ratio="12/9"
        class="ml-sm-16 mt-sm-10" src="https://upload.wikimedia.org/wikipedia/en/thumb/3/30/Zee5_Official_logo.svg/1200px-Zee5_Official_logo.svg.png" 
          width="60" height="60">
          </v-img>
        </v-app-bar-nav-icon><!--logo-->
        
      </v-col>
    
      <v-col cols="9" md="4" sm="6">
        
          <searchbar/>
        
       </v-col>

       <v-col cols="12"
            sm="3"
            md="5" 
          
          class="pl-md-16 pt-2 pl-sm-4" 
          outlined
          tile
          centered
          color="purple darken-4"> <!--right side navigation icons-->
        
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

         
        </v-col>
      </v-row>

      <v-row>
        <v-col cols="12" sm="16" md="12">
         
          <Filter0/>
        
       </v-col>
      </v-row>
      
      <v-row>
        <v-col cols="12" sm="16" md="14">
              <v-card color="purple darken-4">
                <Slide1/> <!--featured taked from components-->
              </v-card>

            </v-col>
            </v-row>

        <v-row>
        <v-col cols="12" sm="16" md="14">
        <v-card 
          color="black"
          class="mt-sm-5 mt-xs-4"
          height="1500">
            <v-carousel hide-delimiters>
            <v-card
            align ="left"
            justify="left"
           
            class="pl-3 pt-3 black">
            <div class=" text-truncate black">
              <h1>Top shows</h1>
            </div> <!--class="pl-16 ml-16 ma-2 mr-n16 black">
            <div class="col-2 ml-16 pl-16 text-truncate black">-->
            </v-card>

              <v-carousel-item>
                <Cards/><!--more series-->
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
            </v-col>
            </v-row>
        
    </v-content>
    <Footer1/>
  </v-responsive>
</template>

<script>

</script>