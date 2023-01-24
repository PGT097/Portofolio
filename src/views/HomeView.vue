<template>
<v-app id="home">
  <NavBar />
  <v-container fluid>
    <div class="head">
      <v-row>
        <v-col cols="5">
          <div style="position:relative" class="mt-16">
            <h1 class="text-grey">Hello,</h1>
            <h1 class="text-white">I'm Cornelia</h1>
            <span class="text-grey"> Painter</span><br />
            <v-btn tile dark class="text-yellow mt-8" variant="outlined"> Contact ME</v-btn>
          </div>
        </v-col>
        <v-col cols="2">
          <div style="position:absolute;z-index: 9999;bottom:0; margin-left:auto; margin-right:auto;left:0;right:0;text-align:center;">
          <v-icon>fas fa-angle-double-down</v-icon>
          </div>
        </v-col>
         <v-col cols="5">
          <div style="position:relative;z-index:9999;opacity:none;" class="mt-16">
            <v-img src="painter2.jpg" contain max-height="300"></v-img>
          </div>
        </v-col>
      </v-row>
    </div>
    <AboutView />
    <ProductsView />
    <GaleryView />
    <ServicesView />
    <ContactView />
  </v-container>
</v-app>
</template>

<script>
import { defineComponent } from 'vue';

// Components
import NavBar from '@/components/NavBar.vue';
import AboutView from '@/views/AboutView.vue';
import GaleryView from './GaleryView.vue';
import ServicesView from './ServicesView.vue';
import ContactView from './ContactView.vue';
import ProductsView from './ProductsView.vue';
export default defineComponent({
  name: 'HomeView',
  setup(){
    return{
      // slider2: 50,
    }
  },

  components: {
    NavBar,
    AboutView,
    GaleryView,
    ServicesView,
    ContactView,
    ProductsView,
  },
});
</script>
<style scoped>
.v-container{
    padding: 16px 0;
}
.head{
  position: relative;
  text-align:center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  width: 100%;
  color:aliceblue;
}
.head:before{
  content: " ";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width:50%;
  background: rgb(0, 0, 0);
  transform: skew(0deg, 6deg);
}
.head:after{
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width:50%;
  background: rgb(9, 9, 9);
  transform: skew(0deg, -6deg);
}






</style>
