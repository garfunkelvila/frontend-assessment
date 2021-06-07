<template>
  <div>
    <v-tabs v-show="!$vuetify.breakpoint.xs" v-model="tab">
      <v-tab
        v-for="item in dataJson"
        :key="item.title"
      >
        {{ item.title }}
      </v-tab>
    </v-tabs>
    <v-tabs-items v-show="!$vuetify.breakpoint.xs" v-model="tab">
      <v-tab-item
        v-for="item in dataJson"
        :key="item.title"
      >
        <v-card flat>
          <v-card-text
            v-html="item.content"
          />
        </v-card>
      </v-tab-item>
    </v-tabs-items>
    <v-expansion-panels v-show="$vuetify.breakpoint.xs" accordion>
      <v-expansion-panel
        v-for="item in dataJson"
        :key="item.title"
      >
        <v-expansion-panel-header>item.title</v-expansion-panel-header>
        <v-expansion-panel-content>
          <div v-html="item.content" />
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </div>
</template>
<script>
export default {
  fetchOnServer: false,
  data () {
    return {
      dataJson: {},
      tab: null
    }
  },
  async fetch () {
    this.dataJson = await this.$axios.get('data.json').then(({ data }) => {
      return data
    })
  }
}
</script>
