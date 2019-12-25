<template>
  <v-app>
    <Drawer />
    <Toolbar />
    <RouterBase />
    <SnackBar />
  </v-app>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

import Drawer from "./core/Drawer.vue";
import Toolbar from "./core/Toolbar.vue";
import RouterBase from "./core/RouterBase.vue";
import SnackBar from "./core/SnackBar.vue";

@Component({
  components: {
    Drawer,
    Toolbar,
    RouterBase,
    SnackBar
  }
})
export default class App extends Vue {}
</script>
