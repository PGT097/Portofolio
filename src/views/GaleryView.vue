<template>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous" />
  <v-col cols="12" sm="12" id="galery">
      <div class="d-flex justify-center mb-6">
        <v-btn color="#0092A5" class="mr-2">All</v-btn>
        <v-btn  class="mr-2" variant="tonal">Painting</v-btn>
        <v-btn  class="mr-2" variant="tonal">Portrets</v-btn>
        <v-btn  class="mr-2" variant="tonal">Landscaping</v-btn>
      </div>
    </v-col>
    <v-col cols="12" class="imgHover" id="galery">
      <v-row class="fill-height" align="center" justify="center">
        <template v-for="(item, i) in items" :key="i">
          <v-col cols="12" md="4">
            <v-hover v-slot="{isHovering, props}">
              <v-card :elevation="isHovering ? 12:2" :class="{'on-hover' : isHovering}" v-bind="props" >
                <v-img :src="item.img" height="225px" cover></v-img>
              </v-card>
            </v-hover>
          </v-col>
        </template>
      </v-row>
    </v-col>
    <v-col cols="12" sm="12">
      <div class="d-flex justify-center mb-6">
        <v-btn color="#0092A5" class="mt-4">Load More</v-btn>
      </div>
    </v-col>

</template>
<script>
export default {
    setup () {
        

        return {
             items:[
        {img: "img01.jpg", category: 'painting'},
        {img: "img02.jpg", category: 'painting'},
        {img: "img03.jpg", category: 'painting'},
        {img: "img04.jpg",},
        {img: "img05.jpg",},
        {img: "img06.jpg",},
        {img: "img07.jpg",},
        {img: "img08.jpg",},
        {img: "img09.jpg",},
           ]
        }
    }
}

</script>

<style  scoped>
.imgHover{
  padding: 0 200px;

}
</style>


    