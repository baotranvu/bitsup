<template>
  <base-header class="base-header" :listItem="listItem"></base-header>

  <router-view />
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";
import BaseHeader from "./components/BaseComponents/Header/BaseHeader.vue";
@Options({
  components: {
    BaseHeader,
  },
})
export default class App extends Vue {
  listItem: unknown = [
    { name: "home", title: "Homepage" },
    { name: "about", title: "About Us" },
    { name: "service", title: "Services" },
    { name: "contact", title: "Contact" },
  ];
}
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.base-header {
  background: #383e4c;
}
</style>
