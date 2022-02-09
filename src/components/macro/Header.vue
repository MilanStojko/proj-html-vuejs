<template>
  <div>
    <HeaderTop />
    <HeaderMain :voci="menunav" class="sticky" />
  </div>
</template>

<script>
import HeaderMain from "../sections/HeaderMain.vue";
import HeaderTop from "../sections/HeaderTop.vue";
import datanav from "../../assets/data/datanav";
export default {
  name: "Header",
  components: { HeaderTop, HeaderMain },
  data() {
    return {
      menunav: datanav,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
</style>