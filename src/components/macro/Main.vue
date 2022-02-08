<template>
  <main>
    <MainJumbo />
    <MainSectionInspire />
  </main>
</template>

<script>
import MainSectionInspire from "../commons/MainSectionInspire.vue";
import MainJumbo from "../sections/MainJumbo.vue";
export default {
  components: { MainJumbo, MainSectionInspire },
  name: "Main",
};
</script>

<style>
</style>