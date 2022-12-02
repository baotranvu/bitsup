<template>
  <div class="box">
    <ul class="tabs">
      <base-header-item></base-header-item>
    </ul>
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
})
export default class BaseHeader extends Vue {}
</script>
