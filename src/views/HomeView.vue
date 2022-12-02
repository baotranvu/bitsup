<template>
  <div class="home">
    <div>
      <base-header></base-header>
    </div>
    <img alt="Vue logo" src="../assets/logo.png" />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src
import BaseHeader from "@/components/BaseComponents/BaseHeader.vue";
@Options({
  components: {
    HelloWorld,
    BaseHeader,
  },
})
export default class HomeView extends Vue {}
</script>
