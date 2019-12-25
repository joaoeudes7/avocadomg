<template>
  <v-navigation-drawer permanent>
    <v-list-item>
      <v-list-item-content>
        <v-list-item-title class="title">AvocatoMG</v-list-item-title>
        <v-list-item-subtitle>Minify Vector XML</v-list-item-subtitle>
      </v-list-item-content>
    </v-list-item>

    <v-divider></v-divider>

    <v-list dense nav>
      <v-list-item v-for="(item, i) in items" :key="i" link>
        <v-list-item-icon>
          <v-icon>{{ item.icon }}</v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>

<script lang='ts'>
import { Component, Prop, Vue } from "vue-property-decorator";

@Component({})
export default class Drawer extends Vue {
  items = [
    { title: "Dashboard", icon: "mdi-view-dashboard" },
    { title: "Photos", icon: "mdi-image" },
    { title: "About", icon: "mdi-help-box" }
  ];
}
</script>

<style lang='scss' scoped>
</style>
