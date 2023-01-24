<template>
<v-col cols="12" class="mt-16" id="about">
      <div>
        <v-row>
          <v-col cols="12" sm="6">
            <div class="egg">
              <v-icon color="black" style="positon:relative; justify-contetnt:align-center;"></v-icon>
              <!-- <v-img src="questioned.jpeg" max-weight="300"></v-img> -->
            </div>
          </v-col>
          <v-col cols="12" sm="6">
            <h5 class="mt-6">About me</h5>
              <div style="width 120px" >
              <v-slider v-model="slider2" color="yellow">
              </v-slider>
              </div>
              <h4 class="mt-n4">I Am a creative painter</h4>
              <h4>And a sincefiction artist</h4>
              <p class="text-orange">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloribus accusantium voluptas facere, aut maxime ullam. Excepturi, asperiores quibusdam iure temporibus magni quae consequuntur perferendis ipsum odio, provident rem error vitae.</p>
              <br/>
              <p class="text-grey">
                Lorem, ipsum.
              </p>
              <v-btn tile dark color="#FF5E00" class="mt-4">
                Download Resume
              </v-btn>
            </v-col>
        </v-row>
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

<style scoped>
.egg{
  display: block;
  margin-left: 100px;
  margin-top: 50px;
  width: 356px;
  height: 300px;
  background-color: #FBDf7e;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
}
</style>