<template>
  <router-link
    class="router-link__title--text-color"
    :to="{ name: item.name }"
    >{{ item.title }}</router-link
  >
</template>
<script lang="ts">
import { Vue } from "vue-class-component";
import { Prop } from "vue-property-decorator";

export default class BaseHeaderItem extends Vue {
  @Prop({ default: { title: "Home", name: "home" } }) item!: {
    title: string;
    name: string;
  };
}
</script>
<style scoped>
.router-link__title--text-color {
  color: #fff;
}
</style>
