<template>
  <v-img
    :src="imgLoc"
    class="page-header"
  >
    <h1 class="px-4">Hello Developer</h1>
    <p class="px-4 text-center">Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
  </v-img>
</template>
<script>
export default {
  props: {
    header: {
      type: String,
      required: true
    },
    subtitle: {
      type: String,
      required: true
    }
  }
}
</script>
