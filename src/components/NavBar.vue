<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container">
                      <v-icon color="yellow" left class="mr-2">fas fa-signature </v-icon>
          <a class="navbar-brand" href="">PetitPeintre</a>
                    
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
                <ul class="navbar-nav ms-auto">
                       <!-- <v-spacer></v-spacer>  -->
                      <v-btn text @click="scroll('home')" class="text-dark">Home</v-btn>
                      <v-btn text @click="scroll('about')">About</v-btn>
                      <v-btn text @click="scroll('products')">Products</v-btn>
                      <v-btn text @click="scroll('galery')">Galery</v-btn>
                      <v-btn text @click="scroll('services')">Services</v-btn>
                      <v-btn text @click="scroll('contact')" >Contact</v-btn>
                </ul>
            </div>
        </div>
    </nav>
</div>
   
</template>

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