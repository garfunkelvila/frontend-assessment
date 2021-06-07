<template>
  <div>
    <v-img
      v-show="$vuetify.breakpoint.xs"
      :src="imageXs"
      class="page-header"
    >
      <h1 class="px-4">
        {{ title }}
      </h1>
      <p class="px-4 text-center">
        {{ subtitle }}
      </p>
      <template #placeholder>
        <v-row
          class="fill-height ma-0"
          align="center"
          justify="center"
        >
          <v-progress-circular
            indeterminate
            color="grey lighten-5"
          />
        </v-row>
      </template>
    </v-img>
    <v-img
      v-show="!$vuetify.breakpoint.xs"
      :src="image"
      class="page-header"
    >
      <h1 class="px-4">
        {{ title }}
      </h1>
      <p class="px-4 text-center">
        {{ subtitle }}
      </p>
      <template #placeholder>
        <v-row
          class="fill-height ma-0"
          align="center"
          justify="center"
        >
          <v-progress-circular
            indeterminate
            color="grey lighten-5"
          />
        </v-row>
      </template>
    </v-img>
  </div>
</template>
<script>
export default {
  props: {
    imageXs: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    },
    title: {
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
<style lang="scss" scoped>
.page-header > ::v-deep .v-responsive__content {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  color: white;
  background: rgba(black, 0.3);
  // backdrop-filter: blur(2px);
}
</style>
