<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-2">
        <div class="university">
          <h2>Avada university</h2>
          <div class="transition">
            <i class="fas fa-home"></i>
            <p>
              Residential Location 9521 Broadsberry Avenue Paddington RC7 9ZA
            </p>
          </div>
          <div class="transition">
            <i class="fas fa-phone-alt"></i>
            <p style="margin-left: 7px">1.800.458.556</p>
          </div>
          <div class="transition">
            <i class="fas fa-envelope"></i>
            <p style="margin-left: 7px"><a href="">info@your-domain.com</a></p>
          </div>
          <div class="transition">
            <i class="fas fa-clock"></i>
            <p style="margin-left: 7px">Monday – Friday: 8:00 AM – 10:00 PM</p>
          </div>
        </div>
      </div>
      <div class="col-2">
        <div class="university">
          <h2>Recent Posts</h2>
          <ul>
            <li
              v-for="(post, index) in postsArr"
              :key="index"
              class="transition separator"
            >
              <span><i :class="post.icon"></i></span>
              <span
                ><a href="">{{ post.text }}</a></span
              >
            </li>
          </ul>
        </div>
      </div>
      <div class="col-2">
        <div class="linkmenu">
          <h2 class="menuti">QUICK LINKS</h2>
          <ul class="menu">
            <li v-for="(link, index) in linksArr" :key="index">
              <p>{{ link.text }}</p>
            </li>
          </ul>
        </div>
      </div>
      <div class="col-2">
        <div class="linkmenu">
          <h2 class="menuti">MENU</h2>
          <ul class="menu">
            <li v-for="(info, index) in navArr" :key="index">
              <a :href="info.src" :class="{ active: info.active }"
                >{{ info.name }} <span v-if="info.new"> new </span>
                <span v-if="info.apply"> apply</span></a
              >
              <div v-if="info.courses"></div>
              <div v-if="info.events"></div>
            </li>
          </ul>
        </div>
      </div>
      <div class="col-4">
        <div>
          <h2>UPCOMING EVENTS</h2>
          <h3 class="events">Upcoming Events</h3>
          <div class="eventcontainer">
            <div class="datecon">
              <div class="month">JUL</div>
              <div class="day">01</div>
            </div>
            <div class="info">
              <h5>Business Seminar</h5>
              <p>July 1 @ 8:00am - 5:00 pm</p>
              <p>United States</p>
            </div>
          </div>
        </div>
        <div>
          <div class="eventcontainer">
            <div class="datecon">
              <div class="month">SEP</div>
              <div class="day">09</div>
            </div>
            <div class="info">
              <h5>Business Seminar</h5>
              <p>July 1 @ 8:00am - 5:00 pm</p>
              <p>United States</p>
            </div>
          </div>
        </div>
        <div class="fix">
          <a href="" class="more">View More...</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterMain",
  props: {
    postsArr: Array,
    linksArr: Array,
    navArr: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
.active {
  color: $orangeText;
}
.more {
  text-decoration: none;
  color: $orangeText;
  padding-top: 20px;
}
.events {
  margin-top: 40px;
}
.eventcontainer {
  display: flex;
  border-bottom: dotted 1px black;
  margin-top: 20px;
  width: fit-content;
  .datecon {
    width: 80px;
    height: 90px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5px;
    background-color: orange;
    margin-bottom: 30px;
    margin-right: 20px;
    .month {
      padding: 8px 18px;
      background-color: $grayBg;
      color: orange;
    }
    .day {
      padding: 8px 15px;
      color: #fff;
      font-weight: bolder;
    }
  }
  .info {
    display: flex;
    flex-direction: column;
    h5 {
      color: $orangeText;
    }
  }
}
h2 {
  font-size: 1.2rem !important;
  font-weight: bold !important;
  text-transform: uppercase;
}
.linkmenu {
  padding: 0 20px;
}
p {
  padding: 0;
}
.container-fluid {
  background-image: url("../../assets/img/university_ft_bg.png");
  background-size: cover;
  height: 700px;
  padding-top: 150px;
}
.university {
  padding: 0 20px 0 30px;
  margin-left: 40px;
  font-size: 15px;
  p {
    display: inline;
  }
  .transition {
    padding-left: 35px;
  }
  a {
    color: $orangeText;
    text-decoration: none;
  }
  .separator {
    border-bottom: dotted 1px black;
    padding: 10px;
    font-weight: 200;
    line-height: 30px;
    font-size: 1rem;
  }
}
svg {
  margin-left: -1.4rem;
  transform: translateX(-1rem);
}
ul {
  padding-left: 0;
  list-style: none;
}
.menuti {
  font-size: 1.3rem;
}
.menu {
  list-style: none;
  display: flex;
  flex-direction: column;
  li {
    padding: 10px 0;
    p {
      color: black;
      padding-left: 5px;
      margin-bottom: 0;
    }
    a {
      text-decoration: none;
      text-transform: uppercase;
      font-weight: normal;
      color: #000;
      transition: 0.5s;
      span {
        color: #fff;
        background-color: #00bcd4;
        padding: 4px;
        font-size: 0.6rem;
        border-radius: 7px;
        position: relative;
        top: -3px;
      }
      &:hover {
        color: $orangeText;
      }
    }
  }
}
</style>