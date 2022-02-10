<template>
  <div class="cleanergray pbot">
    <div class="container">
      <div class="row">
        <div v-for="(news, index) in newsArr" :key="index" class="col-4">
          <div class="newsholder">
            <img :src="news.img" alt="" />
            <div class="newstext">
              <h3>{{ news.title }}</h3>
              <p>
                By <span>{{ news.autor }}</span> | {{ news.date }}
              </p>
              <div>
                <p>
                  <a href="">{{ news.more }}</a>
                </p>
                <p><i :class="news.icon"></i> {{ news.comments }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import datanews from "../../assets/data/datanews";
export default {
  name: "MainNews",
  data() {
    return {
      newsArr: datanews,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
.cleanergray {
  padding-top: 75px;
  background-color: #f7f5f4;
}
.newsholder {
  background-color: #fff;
  img {
    width: 100%;
  }
  .newstext {
    padding: 40px 15px 20px 15px;
    h3 {
      color: $orangeText;
      font-size: 1.5rem;
      font-weight: 400;
    }
    span {
      color: $orangeText;
      cursor: pointer;
    }
    div {
      display: flex;
      justify-content: space-between;
      p {
        color: $orangeText;
        margin-bottom: 0rem !important;
        a {
          text-decoration: none;
          color: $orangeText;
        }
      }
    }
  }
}
</style>