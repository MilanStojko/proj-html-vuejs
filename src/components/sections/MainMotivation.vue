<template>
  <div class="cleaner">
    <div class="container">
      <div class="row">
        <div class="col-7">
          <h3 class="sectiontitle" >WHY CHOOSE AVADA UNIVERSITY?</h3>
          <p>
            We offer a range of training packages in a range of subject areas
            and can offer blended learning opportunities to best meet your
            needs. If sitting in a room with a trainer and having the
            opportunity for discussion with other learners sounds good to you
            then we can offer this. If you prefer to study in your own time and
            at your own speed then one of our world class facilities. <br />
            <br />
            If you prefer to study in your own time and at your own speed then
            one of our e-learning packages may be right up your street. There is
            a third option, which is you like the sound of both but perhaps
            can’t attend all training sessions, this is when blended learning
            comes into its own.
          </p>
        </div>
        <div class="col-5">
          <div class="videocontainer">
            <video controls>
              <source src="../../assets/video/Saratov.mp4" type="video/mp4" />
            </video>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainMotivation",
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
.sectiontitle {
  padding: 60px 0 25px 0;
}
.videocontainer {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  video {
    width: 100%;
    padding: 100px 10px;
  }
}
</style>