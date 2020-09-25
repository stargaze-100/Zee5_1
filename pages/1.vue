<template>
  <div>
    <div class="text-center mb-4">
      <v-btn
        color="pink"
        @click="alert = !alert"
      >
        <v-icon >mdi-filter</v-icon>
        <spacer></spacer>
          <v-title>Filter</v-title>

      </v-btn>
    </div>
    <v-alert
      :value="alert"
      color="Black"
      
      dark
      border="top"
      
      transition="scale-transition"
    >
      Phasellus tempus. Fusce ac felis sit amet ligula pharetra condimentum. In dui magna, posuere eget, vestibulum et, tempor auctor, justo. Pellentesque posuere. Curabitur ligula sapien, tincidunt non, euismod vitae, posuere imperdiet, leo.

      Phasellus nec sem in justo pellentesque facilisis. Phasellus magna. Cras risus ipsum, faucibus ut, ullamcorper id, varius ac, leo. In hac habitasse platea dictumst. Praesent turpis.
    </v-alert>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        alert: true,
      }
    },
  }
</script>