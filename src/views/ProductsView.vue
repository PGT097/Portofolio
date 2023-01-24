<template>
    <div class="text-center mt-4" id="products">
      <h2>What we do</h2>
      <div style="width:120px;margin: 0 auto">
      <v-slider v-model="slider2" color="yellow" >
      </v-slider>
      </div>
    </div>
   <v-col cols="12" class="padd" >
      <div class="first" id="project">
        <v-row>
          <v-col cols="12">
            <div class="child">
              <v-btn icon="fas fa-brush" color="#FFF01F" class="text-white"></v-btn>
              <h3 class="ml-3 mt-4">PAINTER</h3>
              <p class="text-grey ml-3 mt-4 text-caption">
              Lorem, ipsum dolor.
              </p>
            </div>
              <div class="child">
              <v-btn icon="fas fa-mobile" color="#FFF01F" class="text-white"></v-btn>
              <h3 class="ml-3 mt-4">Lanscaping</h3>
              <p class="text-grey ml-3 mt-4 text-caption">
              Lorem, ipsum dolor.
              </p>
            </div>
              <div class="child">
              <v-btn icon="fas fa-camera" color="#FFF01F" class="text-white"></v-btn>
              <h3 class="ml-3 mt-4">Prints</h3>
              <p class="text-grey ml-3 mt-4 text-caption">
              Lorem, ipsum dolor.
              </p>
            </div>
          </v-col>
        </v-row>
        <v-divider></v-divider>
      </div>
    </v-col>
</template>

<script>
export default {
    setup () {
        

        return {
            slider2: 50,
        }
    }
}
</script>

<style  scoped>
.first{
  width: 100%;
  height: 280px;
  text-align:center;
  padding: 2rem 2rem;
}
.child{
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;

}
</style>