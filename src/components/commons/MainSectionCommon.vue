<template>
  <div class="cleaner" >
    <div class="container">
      <div class="centered">
        <div class="logo-container">
          <img src="../../assets/img/page-logo-1.png" alt="" class="logo" />
        </div>
        <h2>{{ titlei }} {{ titlen }}</h2>
        <p>{{ paragi }} {{ paragn }}</p>
        <hr class="linesection" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainSectionInspire",
  props: {
    titlei: String,
    paragi: String,
    titlen: String,
    paragn: String,
    classe: String,
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
</style>