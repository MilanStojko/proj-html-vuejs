<template>
  <div class="fluid">
    <div class="container">
      <div class="spaced">
        <div class="left">
          <img src="../../assets/img/university_logo.png" alt="" class="logo" />
        </div>
        <div class="right">
          <ul>
            <li v-for="(info, index) in voci" :key="index">
              <a :href="info.src"
                >{{ info.name }} <span v-if="info.new"> new </span>
                <span v-if="info.apply"> apply</span></a
              >
              <div v-if="info.courses"></div>
              <div v-if="info.events"></div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderMain",
  props: {
    voci: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
ul {
  list-style: none;
  display: flex;
  li {
    padding: 50px 20px;
    a {
      text-decoration: none;
      text-transform: uppercase;
      font-weight: bold;
      color: #000;
      font-size: 1rem;
      span {
        color: #fff;
        background-color: #00bcd4;
        padding: 4px;
        font-size: 0.6rem;
        border-radius: 7px;
        position: relative;
        top:-2px;
      }
    }
  }
}
</style>