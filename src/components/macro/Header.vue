<template>
  <div>
    <HeaderTop />
    <HeaderMain :voci="menunav" />
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
.sticky-more {
  position: sticky;
  top: 0;
  left: 0;
  right: 0;
}
</style>