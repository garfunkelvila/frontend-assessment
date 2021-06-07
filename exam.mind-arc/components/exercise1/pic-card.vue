<template>
  <v-card
    style="display: flex; flex-direction: column; height: 100%;"
  >
    <v-card-text>
      <v-card>
        <v-img
          src="/images/400x300.png"
        />
      </v-card>
    </v-card-text>
    <v-card-text class="text-center pt-0" style="height: 100%;">
      {{ text }}
    </v-card-text>
    <v-card-text class="justify-center" style="display: flex;">
      <v-btn outlined rounded class="pa-4" style="border: 2px solid black;">
        Read More
      </v-btn>
    </v-card-text>
  </v-card>
</template>
<script>
export default {
  props: {
    text: {
      type: String,
      required: true
    }
  }
}
</script>
