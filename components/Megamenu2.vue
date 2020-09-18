<template>
  <v-card>
    <v-toolbar

      color="black"
      
      dark
      flat
    >
    <!--<v-row>-->
      <v-app-bar-nav-icon>
      <img src="data:image/png;base64,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" 
        width="60" height="60">
      </v-app-bar-nav-icon>

      <!--<v-toolbar-title>Zee5</v-toolbar-title> -->

      <v-spacer></v-spacer>
      
      <v-text-field
        align="center"
        justify="center"
        mdi-magnify
        class="mx-12"
        flat
        hide-details
        label="Search"
        solo-inverted
      ></v-text-field>
      
      <v-btn icon>
        <v-icon>mdi-Account</v-icon>
      </v-btn>
      
      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>

      <template v-slot:extension>
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