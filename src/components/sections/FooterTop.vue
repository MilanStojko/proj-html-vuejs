<template>
  <div class="container-fluid">
    <div class="container">
      <div class="row">
        <div class="col-12 title">
          <div>
            <span>Joing Over</span>
            <span class="number"
              >500,000 Students
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 500 150"
                preserveAspectRatio="none"
              >
                <path d="M8.1,146.2c0,0,240.6-55.6,479-13.8"></path>
              </svg>
            </span>
            <span>Enjoying Avada Education Now</span>
          </div>
          <div class="moto">
            <p>Become Part Of Avada University To Further Your Career.</p>
          </div>
        </div>
      </div>
      <div class="row pbot">
        <div class="col-3">
          <input type="text" name="" placeholder="Name" />
        </div>
        <div class="col-3">
          <input type="text" name="" placeholder="Cognome" />
        </div>
        <div class="col-3">
          <input type="text" name="" placeholder="Telephone" />
        </div>
        <div class="col-3">
          <div class="button">apply now</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterTop",
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/var.scss";
.title {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding-top: 100px;
  padding-bottom: 15px;
  span {
    font-size: 2.3rem;
    color: #fff;
    padding-right: 10px;
    font-weight: 600;
    padding-bottom: 0px;
  }
  .number {
    color: $orangeText !important;
    position: relative;
  }
  svg {
    position: absolute;
    top: 5px;
    right: 10px;
    fill: $orangeText;
    width: 100%;
    height: 50px;
    overflow: visible;
    path {
      stroke: $orangeText;
      stroke-width: 9;
      fill: none;
      stroke-dasharray: 1500;
      stroke-linecap: round;
      stroke-linejoin: round;
      animation: fusion-title-highlight 10s;
    }
  }
  .moto {
    p {
      font-size: 1.5rem;
      padding-top: 0px;
    }
  }
}
input {
  height: 45px;
  padding-left: 10px;
  width: 100%;
  color: #fff !important;
  background-color: #47536c;
  box-shadow: none;
  outline: none;
  border: none;
}
.button {
  height: 45px;
  background-color: $oragneBg;
  padding: 10px;
  text-align: center;
  color: #fff;
  text-transform: uppercase;
  font-weight: 600;
}
</style>