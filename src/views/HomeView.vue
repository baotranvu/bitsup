<template>
  <div class="home">
    <base-banner></base-banner>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import BaseBanner from "@/components/BaseComponents/BaseBaner.vue";

@Options({
  components: {
    BaseBanner,
  },
})
export default class HomeView extends Vue {}
</script>
