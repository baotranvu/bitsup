<template>
  <li>
    <a :href="url">{{ title }}</a>
  </li>
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    title: String,
    url: String,
  },
})
export default class BaseHeaderItem extends Vue {
  title!: string;
  url!: string;
}
</script>
