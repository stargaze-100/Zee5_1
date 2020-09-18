<template>
  <v-card>
    <v-toolbar
      color="#3F0C54"
      dark
      flat
      
    >
    
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Zee5</v-toolbar-title>

      <v-spacer></v-spacer>
      
      <v-text-field
        mdi-magnify
        class="mx-12"
        flat
        hide-details
        label="Search"
        
        solo-inverted
      ></v-text-field>
      
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
      
      
      <template v-slot:extension>

      <v-btn icon>
        <v-icon>mdi-filter</v-icon>
      </v-btn>

        <v-tabs
          v-model="tab"
          centered
          color="pink"
        >
          <v-tabs-slider color="pink"></v-tabs-slider>

          <v-tab v-for="item in items" :key="item" >
            {{ item }}
          </v-tab>
        </v-tabs>
      </template>
    </v-toolbar>

    <v-tabs-items v-model="tab">
      <v-tab-item
        v-for="item in items"
        :key="item"
        
        
      >
       
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
  export default {
    data () {
      return {
        tab: null,
        
        items: [
          'Home', 'Originals', 'Club', 'More',
        ],
      }
    },
  }
  
</script>