<template>
<div>
  <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
      
<!-- 
        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        /> -->
      </div>

      <v-spacer></v-spacer>
<!-- <v-card class="ma-0 pa-0" width="300px"> -->
  <v-text-field
  class="search-bar "
            filled
            label="search"
            append-icon="mdi-magnify"
            hide-details
          ></v-text-field>
        <!-- </v-card> -->
    </v-app-bar>

     

  <v-row class="pa-4">
        <v-col
        v-for="(card,index)   in 12" :key="index"
          cols="12"
          sm="4"
          md="3"
          lg="2"
        >




  <v-card  @click="openDialog" width="250px" height="300px" class="pa-4" outlined> 
      <v-card-subtitle class="px-0 pt-0 pb-1">Title</v-card-subtitle>
      <v-card-Title class="px-0 pt-0 pb-1">Title</v-card-title>
         <v-card-subtitle class=" px-0 pt-0 pb-1">Project Techonology</v-card-subtitle>
         <span v-for="(i,index) in 5" :key="index">java</span>
         <v-card-subtitle class=" px-0 pt-0 pb-1">Techinical_skill_backend</v-card-subtitle>
         <span v-for="(i,index) in 5" :key="index">java</span>
         <v-card-subtitle class=" px-0 pt-0 pb-1">Techinical_skill_Backend</v-card-subtitle>
         <span v-for="(i,index) in 5" :key="index">java</span>
         <v-card-subtitle class="px-0 pt-0 pb-1">Techinical_skill_Backend</v-card-subtitle>
         <span v-for="(i,index) in 5" :key="index">java</span>      
      </v-card>
    </v-col>
      </v-row>

      <v-dialog v-model="dialog" persistent max-width="300" style="position: absolute; top: opx;" class="right-aligned-dialog">
      <v-card class=" pa-4">
        <v-card-subtitle class="px-0 pt-0 pb-1">Title</v-card-subtitle>
        <v-divider></v-divider>
      <v-card-Title class="px-0 pt-0 pb-1">Title</v-card-title>
         <v-card-subtitle class=" px-0 pt-0 pb-1">Project Techonology</v-card-subtitle>
         <span v-for="(i,index) in 5" :key="index">java</span>
         <v-card-subtitle class=" px-0 pt-0 pb-1">Techinical_skill_backend</v-card-subtitle>
         <span v-for="(i,index) in 5" :key="index">java</span>
         <v-card-subtitle class=" px-0 pt-0 pb-1">Techinical_skill_Backend</v-card-subtitle>
         <span v-for="(i,index) in 5" :key="index">java</span>
         <v-card-subtitle class="px-0 pt-0 pb-1">Techinical_skill_Backend</v-card-subtitle>
         <span v-for="(i,index) in 5" :key="index">java</span>      
        <v-card-actions>
          <v-btn color="primary" @click="closeDialog">Close</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
</div>
</template>

<script>
 


  export default {
    name: 'HomeView',
    data() {
    return {
      dialog: true,
    };
  },
  methods: {
    openDialog() {
      this.dialog = true;
    },
    closeDialog() {
      this.dialog = false;
    },
  },
        


  }
</script>
<style>
.search-bar {
  max-width: 300px;

}
.v-dialog {
  position: fixed !important;
  right: 300px;
  top: 0;
  transform: translateX(100%);
}
</style>
