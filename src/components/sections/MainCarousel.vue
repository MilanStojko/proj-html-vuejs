<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-4">
        <div class="course">
          <div class="overlay">
            <h2>courses</h2>
            <hr />
            <span>View More</span>
          </div>
          <img src="../../assets/img/home_courses_section_bg.jpg" alt="" />
        </div>
      </div>
      <div class="col-4">
        <div class="event">
          <div class="overlay">
            <h2>events</h2>
            <hr />
            <span>View More</span>
          </div>
          <img src="../../assets/img/home_events_section_bg.jpg" alt="" />
        </div>
      </div>
      <div class="col-4">
        <div class="news">
          <div class="overlay">
            <h2>latest news</h2>
            <hr />
            <span>View More</span>
          </div>
          <img src="../../assets/img/home_latest_news_section_bg.jpg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainCarousel",
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
.col-4 {
  padding: 0;
}
.course,
.event,
.news {
  height: 800px;
  overflow: hidden;
  position: relative;
  background-color: #fff;
  z-index: 0;
  img {
    transition: 0.5s;
    width: 100%;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    z-index: -1;
  }
  &:hover {
    img {
      transform: scale(1.1);
      opacity: 0.95;
    }
  }
  .overlay {
    height: 100%;
    z-index: 100;
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    h2 {
      text-transform: uppercase;
    }
    hr {
      border-bottom: solid orange 2px;
      width: 100px;
    }
  }
}
</style>