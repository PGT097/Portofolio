<template>
    <v-col cols="12" sm="12" class="px-16" id="contact">
      <v-row>
        <v-col cols="12" sm="4">
          <div class="child">
            <h1>Contact Info</h1>
            <v-btn icon="fas fa-map-marker-alt" class="mt-10" variant="outlined"></v-btn><br />
            <span class="text-caption">My Street, My area dream</span> <br />
            <v-btn icon="fab fa-instagram" class="mt-10" variant="outlined"></v-btn><br />
            <span class="text-caption">peti.tpeintre</span><br />
            <v-btn icon="fas fa-envelope" class="mt-10" variant="outlined"></v-btn><br />
            <span class="text-caption">youremail@gmail.com</span><br />
          </div>
        </v-col>
     
    <v-col cols="12" sm="8">
      <h1 class="mt-8">Send your message</h1>
      <v-divider></v-divider>
      <span class="text-caption">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
        Laboriosam, exercitationem architecto. Pariatur possimus nulla 
        ex eius unde iusto placeat dolorum corrupti eligendi, et ipsam. 
        Dolores natus ab earum voluptatibus blanditiis.
      </span>
      <v-row class="mt-10">
        <v-col cols="12" sm="6">
          <v-text-field label="Name" persistent-hint variant="outlined"></v-text-field>
        </v-col>
        <v-col cols="12" sm="6">
          <v-text-field label="Phone_Number" persistent-hint variant="outlined"></v-text-field>
        </v-col>
      </v-row>
       <v-textarea label="Message" persistent-hint variant="outlined"></v-textarea>
      <v-btn color="teal" class="mt-2">Submit now</v-btn>
    </v-col>
     </v-row>
    </v-col>
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style scoped>
.child{
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;

}
</style>