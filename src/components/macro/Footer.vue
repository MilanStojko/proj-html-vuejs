<template>
  <div>
    <FooterTop class="bluejeans" />
    <FooterMain />
  </div>
</template>

<script>
import FooterMain from "../sections/FooterMain.vue";
import FooterTop from "../sections/FooterTop.vue";
export default {
  components: { FooterTop, FooterMain },
};
</script>

<style lang="scss" scoped>
.bluejeans {
  background-color: #333c4e;
}
</style>