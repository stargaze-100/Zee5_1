<template>
  <v-container class="purple lighten-4">
    <v-row>
      <v-col cols=12>
        <v-hover
        v-slot:default="{ hover }"
        close-delay="200"
      >
          <v-card
            class="pa-md-4 mx-lg-auto"
            color="black"
            
            :elevation="hover ? 12 : 2"
          
            height="350"
            max-width="350"
            >
            <v-card-text class="my-4 text-center title">Hover over me!</v-card-text>
            </v-card>
           </v-hover>
          </v-col>

          <v-col>
          <v-card
            class="pa-md-4 mr-md-5"
            color="black"
            width="250px"
           >
            <v-img src ="https://images.unsplash.com/photo-1505150099521-fde7970bcc3a?ixlib=rb-1.2.1&w=1000&q=80">
              
            </v-img>
          </v-card>
          </v-col>
          <v-col>
           <v-card
              class="pa-md-4 ml-md-auto"
              color="black"
              width="250px"
            >
            <v-card-text>
              Adjust screen size to see spacing changes
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
</template>