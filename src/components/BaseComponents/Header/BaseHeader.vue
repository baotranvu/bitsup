<template>
  <div class="tabs is-centered is-medium is-fullwidth">
    <ul>
      <div v-for="(item, index) in listItem" :key="index">
        <base-header-item :item="item"></base-header-item>
      </div>
    </ul>
  </div>
</template>
<script>
import { Options, Vue } from "vue-class-component";
import { Prop } from "vue-property-decorator";
import BaseHeaderItem from "./BaseHeaderItem.vue";
@Options({
  components: {
    BaseHeaderItem,
  },
})
export default class BaseHeader extends Vue {
  @Prop({ default: [] }) listItem;
}
</script>
<style scoped>
.router-link-active {
  background: #49505f;
}
</style>
