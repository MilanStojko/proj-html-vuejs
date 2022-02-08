<template>
  <div class="fluid">
    <div class="container">
      <div class="spaced">
        <ul>
          <li><i class="fas fa-phone"></i><span>1.800.567.8910</span></li>
          <li><i class="fas fa-envelope"></i><span>Contact Us</span></li>
          <li><i class="fas fa-graduation-cap"></i><span>Alumni</span></li>
          <li><i class="fas fa-university"></i><span>Campus</span></li>
        </ul>
        <ul>
          <li><i class="fab fa-facebook-f"></i></li>
          <li><i class="fab fa-twitter"></i></li>
          <li><i class="fab fa-youtube"></i></li>
          <li><i class="fab fa-instagram"></i></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderTop",
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
.fluid {
  background-color: $oragneBg;
  height: 50px;
  ul {
    display: flex;
    text-align: center;
    text-decoration: none;
    list-style-type: none;
    li {
      padding: 13px 10px;
      color: white;
      font-size: 0.8rem;
      span,
      .fas,
      .fab {
        padding: 10px;
        cursor: pointer;
      }
    }
  }
}
</style>