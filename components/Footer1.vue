<template>
<v-footer 
      absolute
      app
      color="grey-darken" 
      > 
      <span class="white--text">&copy; {{ new Date().getFullYear() }}</span>
      <v-container>
        <v-row>
          <v-col
            cols="12"
            sm="4"
            md="3"
            >
            <h4>ZEE5</h4>
            
            <v-divider></v-divider>
            <br>
            <font size="2">About us<br><br>
            Help centre<br><br>
            Privacy Policy<br><br>
            Parental Control<br><br>
            Terms of use<br><br></font>
          </v-col>
          
          <v-col
            cols="12"
            sm="4"
            md="3"
            >
            <h4>OUR COMMUNITY</h4>
            <v-divider></v-divider>
            <br>
            <font size="2">Originals<br><br>
            News<br><br>
            Shows<br><br>
            Movies<br></br>
            Kids<br><br></font>
          </v-col>
          
            <v-col
            cols="12"
            sm="4"
            md="3"
            >
            <h4>HELP & CONTACT</h4>
            <v-divider></v-divider>
            <br>
            <font size="2"><v-icon>mdi-target</v-icon>Help Center<br><br>
            <v-icon>mdi-email</v-icon>Email Us<br><br>
            <v-icon>mdi-phone</v-icon>080-6824-5911<br><br></font>
          
          </v-col>

          <v-col
            cols="12"
            sm="4"
            md="3"
            >
            <h4>CONTACT US</h4>
            <v-divider></v-divider><br>
            <v-btn icon color="pink" class="mt-16">
              <v-icon medium>mdi-facebook</v-icon>
            </v-btn>
            <v-btn icon color="pink"class="mt-16">
              <v-icon medium>mdi-twitter</v-icon>
            </v-btn>
            <v-btn icon color="pink" class="mt-16">
              <v-icon medium>mdi-instagram</v-icon>
            </v-btn>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>


  </v-app>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-instagram',
      ],
    }),
  }
</script>