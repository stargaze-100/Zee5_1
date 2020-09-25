<template>
  <v-sheet
    height="400"
    class="overflow-hidden"
    style="position: relative;"
  >
    <v-container class="fill-height">
      <v-col
      >
        <v-btn
          color="pink"
          dark
          @click.stop="drawer = !drawer"
        >
          <v-icon>mdi-filter</v-icon>
        <spacer></spacer>
          <v-title>Filter</v-title>
          
        </v-btn>
      </v-col>
    </v-container>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
    >
    <v-treeview
   class="mx-2"
    selectable
    selected-color="deep-purple accent-1"
    :items="items"
  ></v-treeview>
      
    </v-navigation-drawer>
  </v-sheet>
</template>

<script>
  export default {
    data () {
      return {
        drawer: null,
        items: [
        {
          
          name: 'Year:',
          children: [
            { id: 1, name: '2000-2005' },
            { id: 2, name: '2005-2010' },
            { id: 3, name: '2010-2015' },
            { id: 4, name: '2015-2020' },
          ],
        },
        {
          
          name: 'Language:',
          children: [
            { id: 5, name: 'Hindi' },
            { id: 6, name: 'English' },
            { id: 7, name: 'Marathi' },
            { id: 8, name: 'Bengali' },
            { id: 9, name: 'Kanada' },
            { id: 10, name: 'Gujrati' },
            { id: 11, name: 'Tamil' },
            { id: 12, name: 'Telugu' },
          ],
        },
        {
          
          name: 'Status:',
          children: [
            { id: 12, name: 'Airing' },
            { id: 13, name: 'Finished' },
            { id: 14, name: 'On-hold' },
            { id: 15, name: 'Upcoming' },
            
          ],
        },
        {
          
          name: 'Sort:',
          children: [
            { id: 5, name: 'Default' },
            { id: 6, name: 'Alphabetical' },
            { id: 7, name: 'Popularity' },
            { id: 8, name: 'Release date' },
            { id: 8, name: 'Recently updated' },
            { id: 8, name: 'Recently added' },
            { id: 8, name: 'Most watched' },
            
          ],
        },
        {
          
          name: 'Sub/Dub:',
          children: [
            { id: 5, name: 'Subbed' },
            { id: 6, name: 'Dubbed' },
            
          ],
        },

        {
          
          name: 'Genre:',
          children: [
            { id: 5, name: 'Action' },
            { id: 6, name: 'Comedy' },
            { id: 7, name: 'Crime' },
            { id: 8, name: 'Drama' },
            { id: 8, name: 'Fantasy' },
            { id: 8, name: 'Historical' },
            { id: 8, name: 'Horror' },
            { id: 8, name: 'Military' },
            { id: 8, name: 'Mystery' },
            { id: 8, name: 'Romance' },
            { id: 8, name: 'Thriller' },
            { id: 8, name: 'School' },
            
          ],
        },

      ],
      }
      
    },
  }
</script>