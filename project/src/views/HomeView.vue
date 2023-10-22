<template>
<div>
  <v-card width="250px" height="300px" class="" outlined> 
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
</div>
</template>

<script>
 


  export default {
    name: 'HomeView',


  }
</script>
