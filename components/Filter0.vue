<template>
  <v-row justify="center">
    <v-dialog
      v-model="dialog"
      scrollable
      
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="pink"
          dark
          v-bind="attrs"
          v-on="on"
        >
          <v-icon>mdi-filter</v-icon><!--Is a dialogue box originally-->
        <spacer></spacer>
          <v-list-item-title>Filter</v-list-item-title>
        </v-btn>
      </template>
      <v-card>
        
        <v-row>
        <v-col>
         <!--Checkboxes in order to filter content-->
        <v-title>Year</v-title>
        <v-divider></v-divider>
            <v-checkbox
            color="pink"
              label="2001-2005"
              
            ></v-checkbox>
            <v-checkbox
              label="2006-2010"
              color="pink"
            ></v-checkbox>
            <v-checkbox
            color="pink"
              label="2011-2015"
            ></v-checkbox>
            <v-checkbox
            color="pink"
              label="2016-2020"
            ></v-checkbox>
         </v-col>

        <v-col>
        <v-title>Language</v-title>
        <v-divider></v-divider>
            <v-checkbox
              label="Hindi"
              color="pink"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="English"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Bengali"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Gujrati"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Tamil"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Telugu"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Kanada"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Marathi"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Punjabi"
            ></v-checkbox>
        </v-col>

        <v-col>
        <v-title>Status</v-title>
        <v-divider></v-divider>
            <v-checkbox
              label="Airing"
              color="pink"
            ></v-checkbox>
            <v-checkbox
              label="Finished"
              color="pink"
            ></v-checkbox>
            <v-checkbox
              label="On-hold"
              color="pink"
            ></v-checkbox>
            <v-checkbox
              label="Upcoming"
              color="pink"
            ></v-checkbox>
        </v-col>

        <v-col>
        <v-title>Sort</v-title>
        <v-divider></v-divider>
            <v-checkbox
            color="pink"
              label="Default"
            ></v-checkbox>
            <v-checkbox
            color="pink"
              label="Recently added"
            ></v-checkbox>
            <v-checkbox
            color="pink"
              label="Recently updated"
            ></v-checkbox>
            <v-checkbox
            color="pink"
              label="Popularity"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Most watched"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Release date"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Alphabetical"
            ></v-checkbox>
        </v-col>

        <v-col>
        <v-title>Sub/dub</v-title>
        <v-divider></v-divider>
            <v-checkbox
            color="pink"
              label="Subbed"
            ></v-checkbox>
            <v-checkbox
            color="pink"
              label="Dubbed"
            ></v-checkbox>
            
        </v-col>
        <v-col>
        <v-title>Genre</v-title>
        <v-divider></v-divider>
            <v-checkbox
            color="pink"
              label="Action"
            ></v-checkbox>
            <v-checkbox
            color="pink"
              label="Comedy"
            ></v-checkbox>
            <v-checkbox
            color="pink"
              label="Crime"
            ></v-checkbox>
            <v-checkbox
            color="pink"
              label="Drama"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Fantasy"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Historical"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Horror"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Military"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Mystery"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Romance"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="Thriller"
            ></v-checkbox>
             <v-checkbox
             color="pink"
              label="School"
            ></v-checkbox>
        </v-col>

        </v-row>
        <!--choice of filtering or not-->
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            color="deep-purple accent-1"
            text
            @click="dialog = false"
          >
            Filter
          </v-btn>
          <v-btn
            color="deep-purple accent-1"
            text
            @click="dialog = false"
          >
            Cancel
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>

    <spacer> </spacer>

    <!--the other navigation menu icons-->
     <v-btn>
      
      <v-icon>mdi-home</v-icon>
      <spacer></spacer>
      <span>Home</span>
    </v-btn>

    <v-btn>
      
      <v-icon>mdi-television-play</v-icon>
      <spacer></spacer>
      <span>Originals</span>
    </v-btn>

    <v-btn>
     
      <v-icon>mdi-book</v-icon>
      <spacer></spacer>
       <span>Club</span>
    </v-btn>

    
    <v-btn>
     
      <v-icon>mdi-apps</v-icon>
      <spacer></spacer>
       <span>More</span>
    </v-btn>
    
  </v-row>
</template>

<script>
  export default {
    data () {
      return {
        dialogm1: '',
        dialog: false,
      }
      
    },
  }
</script>