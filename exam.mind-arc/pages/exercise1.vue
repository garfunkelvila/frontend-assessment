<template>
  <div>
    <header-image
      image="/images/1920x650.png"
      image-xs="/images/600x600.png"
      title="Hello Developer!"
      subtitle="Lorem ipsum dolor sit amet, consectetur adipiscing elit"
    />
    <v-container>
      <v-row>
        <v-col cols="12" sm="4">
          <pic-card
            text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
          />
        </v-col>
        <v-col cols="12" sm="4">
          <pic-card
            text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua."
          />
        </v-col>
        <v-col cols="12" sm="4">
          <pic-card
            text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco."
          />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
import PicCard from '../components/exercise1/pic-card.vue'
import HeaderImage from '../components/exercise1/header-image.vue'

export default {
  components: {
    PicCard,
    HeaderImage
  }
}
</script>
