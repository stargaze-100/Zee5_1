<template fluid>
  <v-row align="center">
  <v-col align="center">
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
        <br></br>
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
     </v-col >

    <spacer> </spacer>
    <v-col class=""
    align="center">
    <!--the other navigation menu icons-->
     <v-btn color = "black">
      
      <v-icon>mdi-home</v-icon>
      <spacer></spacer>
      <span>Home</span>
    </v-btn>
    </v-col>

    <v-col align="center">
    <v-btn color = "black">
      
      <v-icon>mdi-television-play</v-icon>
      <spacer></spacer>
      <span>Originals</span>
    </v-btn>
    </v-col>

    <v-col class=""
    align="center">
    <v-btn color = "black">
     
      <v-icon>mdi-book</v-icon>
      <spacer></spacer>
       <span>Club</span>
    </v-btn>
    </v-col>
    
    <v-col>
    <v-menu
      v-for="([text, rounded], index) in btns"
      :key="text"
      :rounded="rounded"
      offset-y
    >
      <template v-slot:activator="{ attrs, on }">
        <v-btn
          color="black"
          class="white--text ma-8"
          v-bind="attrs"
          v-on="on"
        >
         <v-icon>mdi-cards</v-icon>
          More
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="item in items"
          :key="item"
          link
        >
          <v-list-item-title v-text="item"></v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
  </v-col>
    
  </v-row>
</template>

<script>
  export default {
    data: () => ({
      btns: [
        
        ['Large', 'lg'],
        
      ],
      colors: ['deep-purple accent-4', 'error', 'teal darken-1'],
      items: ['Movie','Show', 'News', 'Kids','Games', 'Music', 'Live TV', 'Stories'],
     
    }),
  }
</script>