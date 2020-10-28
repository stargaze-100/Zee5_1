<template>
  <v-footer class="mt-lg-16 mt-md-16" color="black">
    <v-row>
      <v-col cols="12" sm="2" md="2" lg="2" xs="2">
        <h4>About Us</h4>
        <!-- header tag gives the word a specific size -->

        <br />
        <!-- br tag is used to create specific margins between a column  -->
        <v-divider></v-divider><br />
        <!-- divider give a small margin between two words  -->
        <h4>Help Center</h4>
        <br />
        <v-divider></v-divider><br />
        <h4>Privacy Policy</h4>
        <br />
        <v-divider></v-divider><br />
        <h4>Parental Control</h4>
        <br />
        <v-divider></v-divider><br />
        <h4>Terms Of Use</h4>
      </v-col>

      <v-col cols="12" sm="2" md="2" lg="2" xs="2">
        <h4>ZEE5 Original</h4>
        <br />
        <font size="2"
          >State of Seige: 26/11
          <br />
          XXX <br />
          Mentalhood<br />
          Rangbaaz<br />
          <br
        /></font>
        <v-divider></v-divider>
        <br />
        <h4>Premium Zee5 Originals</h4>
        <br />
        <font size="2">Mafia <br />Reject <br />Lalbazar <br />Rangbaaz</font>
      </v-col>

      <v-col cols="12" md="2" lg="2" sm="2" xs="2">
        <h4>Club Original</h4>
        <br />
        <font size="2"
          >Fitrat<br />
          Jamai 2.0<br />
          Karrle Tu Fir Mohabbat<br />
          Daarish<br /><br
        /></font>
        <v-divider></v-divider>
        <br />
        <h4>Premium Zee5 Originals</h4>
        <br />
        <font size="2">Mafia <br />Reject <br />Lalbazar <br />Rangbaaz</font>
      </v-col>

      <v-col cols="12" md="2" lg="2" sm="2" xs="2">
        <h4>ZEE5 Premium Movies</h4>
        <br />
        <font size="2"
          >Ateet<br />
          Commando<br />
          Simbba<br />
          Uri:The Surgical Strike<br
        /></font>
        <br /><v-divider></v-divider><br />
        <h3>Download Apps</h3>
        <br /><br />
        <h3>Connect With Us</h3>
      </v-col>

      <v-col cols="12" md="2" lg="2" sm="2" xs="2">
        <h5>TV Shows</h5>
        <br />
        <font size="2"
          >Kumkum Bhagya<br />
          Kundali Bhagya<br />
          Kehna ko Humsafar Hai<br />
          Tuzhse hai Raabta<br /></font
        ><br /><br />
       
        <br />
        <v-row>
          <!-- v-icon uses icons from vuetify library -->
          <v-btn color="black">
          <v-icon medium>mdi-youtube </v-icon>
          </v-btn>
          <v-spacer></v-spacer>
          <v-btn color="black">
          <v-icon medium>mdi-instagram </v-icon>
          </v-btn>
          <v-spacer></v-spacer>
          <v-btn color="black">
          <v-icon medium>mdi-facebook </v-icon>
          </v-btn>
          <v-spacer></v-spacer>
          <v-btn color="black">
          <v-icon medium>mdi-twitter </v-icon>
          </v-btn>
          <v-spacer></v-spacer>
        </v-row>
      </v-col>

      <v-col cols="12" md="2" lg="2" sm="2" xs="2">
        <h4>News</h4>
        <br />
        <font size="2"
          >Corona Outbreak<br />
          Today's Headline<br />
          Trending Topics<br />
          Entertainment News<br /></font
        ><br /><br />
        <v-img src="AppStore.jpg"> </v-img>

        <v-row> </v-row>
      </v-col>
    </v-row>
  </v-footer>
</template>