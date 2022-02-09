<template>
  <main>
    <MainJumbo />
    <MainSectionInspire />
    <MainMotivation />
    <MainValues />
  </main>
</template>

<script>
import MainSectionInspire from "../commons/MainSectionInspire.vue";
import MainJumbo from "../sections/MainJumbo.vue";
import MainMotivation from "../sections/MainMotivation.vue";
import MainValues from '../sections/MainValues.vue';
export default {
  components: { MainJumbo, MainSectionInspire, MainMotivation, MainValues },
  name: "Main",
};
</script>

<style>
</style>