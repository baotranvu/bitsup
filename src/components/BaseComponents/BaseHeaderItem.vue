<template>
  <li>
    <a href="/">Home</a>
  </li>
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    Item: Object,
  },
})
export default class BaseHeaderItem extends Vue {}
</script>
