<template>
  <div class="fluid-gray m200">
    <svg
      class="fusion-big-triangle-candy"
      xmlns="http://www.w3.org/2000/svg"
      version="1.1"
      width="100%"
      height="100"
      viewBox="0 0 100 100"
      preserveAspectRatio="none"
      style="padding: 0"
      fill="rgba(255,255,255,1)"
    >
      <path d="M-1 -1 L50 99 L101 -1 Z"></path>
    </svg>
    <div class="container">
      <div class="row">
        <div class="col-6">
          <h3>WORLD CLASS FACILITIES</h3>
          <p>
            Avada University is devoted to excellence in teaching, learning, and
            research, and developing leaders in many disciplines who make a
            difference globally.
          </p>
          <div class="info">
            <p><i class="fas fa-globe"></i></p>
            <h5>International focus</h5>
            <p>- our students come from across the globe</p>
          </div>
          <div class="info">
            <p><i class="fas fa-graduation-cap"></i></p>
            <h5>Residential courses</h5>
            <p>- we encourage learning and growth</p>
          </div>
          <div class="info">
            <p><i class="far fa-address-book"></i></p>
            <h5>People not profits</h5>
            <p>- education is a right not a privilege</p>
          </div>
          <p>
            If you prefer to study in your own time and at your own speed then
            one of our e-learning packages may be right up your street.
          </p>
        </div>
        <div class="col-6">
          <h3 class="tvalues">OUR VALUES</h3>
          <div v-for="(elem, index) in values" :key="index" class="values">
            <i :class="elem.basic"></i>
            <h6 @click="inActive = !inActive">{{ elem.name }}</h6>
            <p v-if="!inActive">{{ elem.text }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import datavalues from "../../assets/data/datavalues";
export default {
  name: "MainValues",
  data() {
    return {
      values: datavalues,
      inActive: true,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
.fluid-gray {
  background-color: $grayBg;
  .fusion-big-triangle-candy {
    margin-bottom: 100px;
  }
  p {
    margin-bottom: 0.5rem;
  }
  svg {
    color: $orangeText;
  }
  .info {
    display: flex;
    align-items: center;
    p {
      padding-right: 20px;
    }
    h5 {
      padding-right: 3px;
    }
  }
  .values {
    display: flex;
    min-height: 60px;
    height: fit-content;
    align-items: center;
    align-content: center;
    background-color: $whiteBg;
    margin-bottom: 10px;
    width: 100%;
    h6,
    svg {
      font-weight: 600;
      font-size: 1.4rem;
      padding: 0 10px;
      color: $orangeText;
    }
    svg {
      transform: translateY(-4px);
    }
    p {
      display: flex;
      flex-direction: column;
    }
  }
}
.m200 {
  padding-bottom: 150px;
}
</style>