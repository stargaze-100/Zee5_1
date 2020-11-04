<template >
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->

    <!-- Body -->
    <v-content light>
      <nuxt /> 
    </v-content>
    
    <!-- Footer -->
    <v-footer style="background-color:#2B1031" app>
      <!--<span class="white--text">&copy; {{ new Date().getFullYear() }}</span>-->
    </v-footer>

  </v-app>
</template>

<script>
export default {}
</script>

<style> 
  .white--text {
    border: 1px solid;
  }

   #inspire {
    background-color:"purple darken-4";
  }
</style>