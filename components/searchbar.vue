 <template>
        <v-card
          class="mr-6"
          tile
          centered
          <v-text-field
            class="pr-sm-10 mt-3 pl-md-1"
            solo
            rounded
             v-model="message2"
            hide-details
            label="Search"
            solo-inverted
            
            append-icon="mdi-magnify"><!--Adds search icon in the text area-->
          </v-text-field>
        </v-card>
       
        </template>