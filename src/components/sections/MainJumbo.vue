<template>
  <section>
    <div class="container jumbotext">
      <h1>Inspiring Tomorrows Leaders</h1>
      <p>The Future Belongs To Those Who See Possibilities Today</p>
      <div class="buttons">
        <div class="button orange">find a course</div>
        <div class="button azure">apply now</div>
      </div>
    </div>
    <div class="jumbotron"></div>
  </section>
</template>

<script>
export default {
  name: "MainJumbo",
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
.jumbotron {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background-image: url("../../assets/img/home_main_slider_bg.jpg");
  background-size: cover;
  z-index: -1;
}
.jumbotext {
  padding: 250px 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: $textWhite;
  h1 {
    font-size: 4.5rem;
  }
  p {
    font-size: 1.4rem;
    color: #fff;
  }
  .buttons {
    display: flex;
    gap: 20px;
    .button {
      padding: 10px 25px;
      border-radius: 2px;
      text-transform: uppercase;
      cursor: pointer;
      font-size: 0.9rem;
      letter-spacing: 2px;
      font-weight: 600;
      transition: 1s;
    }
    .orange {
      background-color: $oragneBg;
      &:hover {
        background-color: $azureBg;
      }
    }
    .azure {
      background-color: $azureBg;
      &:hover {
        background-color: #fff;
        color: #000;
      }
    }
  }
}
</style>