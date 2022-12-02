<template>
  <div>
    <div class="tabs is-centered is-boxed is-medium">
      <ul>
        <base-header-item></base-header-item>
        <base-header-item></base-header-item>
        <base-header-item></base-header-item>
        <base-header-item></base-header-item>
      </ul>
    </div>
  </div>
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";
import BaseHeaderItem from "./BaseHeaderItem.vue";
@Options({
  props: {
    listItem: Array,
  },
  components: {
    BaseHeaderItem,
  },
  data() {
    return {
      Item: {
        title: "Home",
        url: "/",
      },
    };
  },
})
export default class BaseHeader extends Vue {}
</script>
