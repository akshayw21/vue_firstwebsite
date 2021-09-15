
<template>
  <v-card
    elevation="24"
    max-width="1200"
    class="mx-auto"
  >
    <v-system-bar lights-out></v-system-bar>
    <v-carousel
      :continuous="false"
      :cycle="cycle"
      :show-arrows="false"
      hide-delimiter-background
      delimiter-icon="mdi-minus"
      height="500"
    >
      <v-carousel-item
        v-for="(slide, i) in slides"
        :key="i"
      > 
       <v-img :src="slide.imageurl"></v-img>
      </v-carousel-item>
    </v-carousel>
    <v-list two-line>
      <v-list-item>
        <v-list-item-avatar>
          <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
        </v-list-item-avatar>
        <v-list-item-action>
          <v-switch
            v-model="cycle"
            label="Cycle Slides"
            inset
          ></v-switch>
        </v-list-item-action>
      </v-list-item>
    </v-list>
  </v-card>
</template>


<script>
export default {
      data () {
      return {
        
        cycle: false,
        slides: [
          {imageurl: 'https://image.shutterstock.com/image-illustration/snow-falling-stock-image-black-260nw-1519161953.jpg', title:'first image'},
          {imageurl: 'https://image.shutterstock.com/image-illustration/abstract-blue-red-smoke-steam-260nw-1468643051.jpg', title:'first image'},
          {imageurl: 'https://image.shutterstock.com/image-illustration/snow-falling-stock-image-black-260nw-1519161953.jpg', title:'first image'},
          {imageurl: 'https://image.shutterstock.com/image-illustration/snow-falling-stock-image-black-260nw-1519161953.jpg', title:'first image'},
          {imageurl: 'https://image.shutterstock.com/image-illustration/snow-falling-stock-image-black-260nw-1519161953.jpg', title:'first image'},
        ],
      }
    }

}
</script>

<style>

</style>