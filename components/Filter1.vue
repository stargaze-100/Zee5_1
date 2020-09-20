<template>
  <v-card
    class="mx-auto"
    width="300"
  >
    <v-list>
    <!--
      <v-list-item>
        <v-list-item-icon>
          <v-icon>mdi-filter</v-icon>
        </v-list-item-icon>

        <v-list-item-title>FIlter</v-list-item-title>
      </v-list-item>
    -->
      <v-list-group
        mdb-icon  icon="filter" 
        value="true"
        
       >
        <template v-slot:activator>
        <v-icon>mdi-filter</v-icon>
        <spacer></spacer>
          <v-list-item-title>Filter</v-list-item-title>
        </template>

        <v-list-group
          no-action
          sub-group
          value="true"
          
         >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Year</v-list-item-title>
            </v-list-item-content>
          </template>

          <v-list-item
            v-for="(admin, i) in admins"
            :key="i"
            link
            
          >
            <v-list-item-title v-text="admin[0]" ></v-list-item-title>
            <v-list-item-icon>
              <v-icon v-text="admin[1]"
              
              ></v-icon>
            </v-list-item-icon>
          </v-list-item>
        </v-list-group>

        <v-list-group
          sub-group
          no-action
         >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Language</v-list-item-title>
            </v-list-item-content>
          </template>
          <v-list-item
            v-for="(crud, i) in cruds"
            :key="i"
            @click=""
          >
            <v-list-item-title v-text="crud[0]"></v-list-item-title>
            <v-list-item-action>
              <v-icon v-text="crud[1]"></v-icon>
            </v-list-item-action>
          </v-list-item>
        </v-list-group>
      

        <v-list-group
          sub-group
          no-action
         >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Status</v-list-item-title>
            </v-list-item-content>
          </template>
          <v-list-item
            v-for="(a, i) in as"
            :key="i"
            @click=""
          >
            <v-list-item-title v-text="a[0]"></v-list-item-title>
            <v-list-item-action>
              <v-icon v-text="a[1]"></v-icon>
            </v-list-item-action>
          </v-list-item>
        </v-list-group>
      

        <v-list-group
          sub-group
          no-action
         >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Sort</v-list-item-title>
            </v-list-item-content>
          </template>
          <v-list-item
            v-for="(sor, i) in sors"
            :key="i"
            @click=""
          >
            <v-list-item-title v-text="sor[0]"></v-list-item-title>
            <v-list-item-action>
              <v-icon v-text="sor[1]"></v-icon>
            </v-list-item-action>
          </v-list-item>
        </v-list-group>
     

         <v-list-group
          sub-group
          no-action
         >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Sub/Dub</v-list-item-title>
            </v-list-item-content>
          </template>
          <v-list-item
            v-for="(title, i) in titles"
            :key="i"
            @click=""
          >
            <v-list-item-title v-text="title[0]"></v-list-item-title>
            <v-list-item-action>
              <v-icon v-text="title[1]"></v-icon>
            </v-list-item-action>
          </v-list-item>
        </v-list-group>
      

       <v-list-group
          sub-group
          no-action
         >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Genre</v-list-item-title>
            </v-list-item-content>
          </template>
          <v-list-item
            v-for="(genre, i) in genres"
            :key="i"
            @click=""
          >
            <v-list-item-title v-text="genre[0]"></v-list-item-title>
            <v-list-item-action>
              <v-icon v-text="genre[1]"></v-icon>
            </v-list-item-action>
          </v-list-item>
       </v-list-group>
     </v-list-group>
    

    </v-list>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      admins: [
        ['2000-2005',],
        ['2006-2010',],
        ['2011-2015',],
        ['2015-2020',],
      ],
      cruds: [
        ['English',],
        ['Hindi', ],
        ['Bengali',],
        ['Marathi',],
        ['Gujrati',],
        ['Malyali',],
        ['Punjabi',],
        ['Tamil',],
      ],
       as: [
        ['Airing',],
        ['Ongoing', ],
        ['Completed',],
        ['Pending',],
        
      ],
       sors: [
        ['Default',],
        ['Recently added', ],
        ['Recently updated',],
        ['Popularity',],
        ['Alphabetical',],
        ['Most watched',],
        ['Release date',],
       ],  
       titles: [
        ['Dubbed',],
        ['Subbed', ],
       ],
        genres: [
        ['Romance',],
        ['Thriller', ],
        ['ACtion', ],
        ['Comedy', ],
        ['Crime', ],
        ['Drama', ],
        ['Fantasy', ],
        ['Historical', ],
        ['Horror', ],
        ['Military', ],
        ['Mystery', ],
        ['School', ],
       ],
      
    }),
  }
</script>