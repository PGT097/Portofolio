<template>
  <v-app-bar app color="teal" dark flat class="px-12">
    <v-btn>
        <v-icon color="yellow" left class="mr-2">fas fa-signature </v-icon>PetitPeintre
    </v-btn>
    <v-spacer></v-spacer>
    <v-btn text @click="scroll('home')" class="text-yellow">Home</v-btn>
    <v-btn text @click="scroll('about')">About</v-btn>
    <v-btn text @click="scroll('products')">Products</v-btn>
    <v-btn text @click="scroll('galery')">Galery</v-btn>
    <v-btn text @click="scroll('services')">Services</v-btn>
    <v-btn text @click="scroll('contact')" >Contact</v-btn>
    </v-app-bar>
</template>ß

<script>
export default {
   methods:{
    scroll(refName) {
        const element = document.getElementById(refName);
        element.scrollIntoView({behavior: "smooth"});
    }
   }
}
</script>

<style  scoped>

</style>