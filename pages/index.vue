<template>
<v-container fluid>
  <v-content style="background-color:#241025" centered>
  <v-footer 
  
  style="background-color:#1D0E1E">
    <v-row>
    
      <v-col cols="2" sm="2" md="3"> 
        
          <v-app-bar-nav-icon disabled>
        <v-img 
        class="ml-sm-16 mt-sm-10" src="zee5logo.png" 
          width="100" height="100">
          </v-img>
        </v-app-bar-nav-icon><!--logo-->
        
      </v-col>
    
      <v-col cols="9" md="6" sm="7">
        
          <searchbar/>
        
       </v-col>

       <v-col cols="10"
            sm="3"
            md="3" 
          class="pt-6 pl-12 d-flex flex-row-reverse" 
          
          
          tile
          
          > <!--right side navigation icons-->
        
           <v-btn fab small class= "mt-1 ma-2" color = "purple lighten-3">
            <v-icon color ="black">mdi-pencil</v-icon> 
          </v-btn>

           <v-btn fab small class= "mt-1 ma-2" color = "purple lighten-3">
            <v-icon color ="black">mdi-wrench</v-icon>
          </v-btn>
          
          <v-btn fab small class= "mt-1 ma-2" color = "purple lighten-3">
            <v-icon color ="black">mdi-account</v-icon>
          </v-btn>
          
          <v-btn fab small class= "mt-1 ma-2" color = "purple lighten-3">
           <v-icon color ="black">mdi-format-list-bulleted-square</v-icon>
          </v-btn>

         
        </v-col>
      </v-row>
      </v-footer>
     <v-divider></v-divider>
     <v-footer  style="background-color:#241025">
      <v-row>
        <v-col cols="12" sm="16" md="12" xs="12">
         
          <Filter0/>
        
       </v-col>
      </v-row>
      </v-footer>
      
      <v-row>
        <v-col cols="12" sm="16" md="14">
              <v-card color="purple darken-4">
                <Slide1/> <!--featured taked from components-->
              </v-card>

            </v-col>
            </v-row>

        <v-row>
        <v-col cols="12" sm="16" md="14" 
        >
        
            <v-scroll>
            <v-card style="background-color:#241025">
            <h1>Top shows</h1>
            <v-divider></v-divider>
            <v-carousel hide-delimiters>
              <v-carousel-item >
                <Cards/><!--more series-->
              </v-carousel-item>
              <v-carousel-item>
                <Card2/>
              </v-carousel-item>
            </v-carousel>
            </v-card>
            <v-card style="background-color:#241025">
            <h1>Recommended</h1>
            <v-divider></v-divider>
              <v-carousel hide-delimiters>
              <v-carousel-item>
                <Card4/>
              </v-carousel-item>
              <v-carousel-item>
                <Card3/>
              </v-carousel-item>
            </v-carousel>
            </v-card>
            <v-card style="background-color:#241025">
            <h1>Thriller</h1>
            <v-divider></v-divider>
              <v-carousel hide-delimiters>
              <v-carousel-item>
                <Card3/>
              </v-carousel-item>
              <v-carousel-item>
                <Card2/>
              </v-carousel-item>
            </v-carousel>
            </v-card>
            <v-card style="background-color:#241025">
            <h1>Comedy</h1>
            <v-divider></v-divider>
              <v-carousel hide-delimiters>
              <v-carousel-item>
                <Card2/>
              </v-carousel-item>
              <v-carousel-item>
                <Card4/>
              </v-carousel-item>
            </v-carousel>
            </v-card>
          </v-scroll>
            <v-card>
            <Footer2/>
            </v-card>
            
            
            </v-col>
           
            
         </v-row>
         
    </v-content>
    
  </v-container>
  
</template>

<script>

</script>