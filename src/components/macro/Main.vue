<template>
  <main>
    <MainJumbo />
    <MainSectionCommon :titlei="inspireh" :paragi="inspirep" />
    <MainMotivation />
    <MainValues />
    <MainCarousel />
    <MainSectionCommon :titlen="newsh" :paragn="newsp" />
    <MainNews />
  </main>
</template>

<script>
import MainSectionCommon from "../commons/MainSectionCommon.vue";
import MainCarousel from "../sections/MainCarousel.vue";
import MainJumbo from "../sections/MainJumbo.vue";
import MainMotivation from "../sections/MainMotivation.vue";
import MainNews from "../sections/MainNews.vue";
import MainValues from "../sections/MainValues.vue";
export default {
  name: "Main",
  components: {
    MainJumbo,
    MainSectionCommon,
    MainMotivation,
    MainValues,
    MainCarousel,
    MainNews,
  },
  data() {
    return {
      inspireh: "Inspired By Excellence & Innovation",
      inspirep:
        "We offer a wide range of high quality of teaching and extra curricular activities",
      newsh: "Today’s Univeristy News",
      newsp:
        "Covering Topics From Classes To Politics And Student Organization Events.",
    };
  },
};
</script>

<style lang="scss" scoped>
</style>