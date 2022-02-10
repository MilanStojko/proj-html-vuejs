<template>
  <div>
    <FooterTop class="bluejeans" />
    <FooterMain :postsArr="dataposts" :linksArr="datalinks" :navArr="navdata" />
  </div>
</template>

<script>
import FooterMain from "../sections/FooterMain.vue";
import FooterTop from "../sections/FooterTop.vue";
import { posts, links } from "../../assets/data/datafooter";
import datanav from "../../assets/data/datanav"
export default {
  components: { FooterTop, FooterMain },
  data() {
    return {
      dataposts: posts,
      datalinks: links,
      navdata : datanav,
    };
  },
};
</script>

<style lang="scss" scoped>
.bluejeans {
  background-color: #333c4e;
}
</style>