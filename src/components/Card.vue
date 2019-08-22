<template>
  <div class="float-left ml-12 mt-12">
    <v-card
      class="mx-auto"
      :elevation="elevation"
      :width="width"
      :height="height"
    >
      <v-row
        class="py-4 pl-4"
      >
        <v-col class="shrink ml-2 mb-2">
          <v-img
            class="white--text"
            height="500"
            width="500"
            src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
          >
            <v-card-title class="align-end fill-height">I'm a title</v-card-title>
          </v-img>
        </v-col>
        <v-col>
          <v-card-text>I'm card text</v-card-text>
          <v-card-actions>
            <v-btn icon>
              <v-icon>mdi-heart</v-icon>
            </v-btn>
            <v-btn text>Click</v-btn>
            <v-btn outlined>Click</v-btn>
          </v-card-actions>
        </v-col>
      </v-row>
    </v-card>
  </div>
</template>

<script>
export default {
  data(){
    return{
      elevation: 24,
      width: 1500,
      height: 550,
    }
  }
}
</script>

<style>

</style>