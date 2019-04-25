<template>
  <div class="container">
      <div class="main_wrapper">
          <div class="logo">
              <img class="mikanLogo" src="../static/mikan_logo.png" />
              <img class="tunaLogo" src="../static/tuna_logo.png" />
          </div>
          <div class="sub_wrapper">
              <div class="aboutus">ABOUT US</div>
              <div class="img_wrapper">
              </div>
          </div>
      </div>
  </div>
</template>

<script>

export default {
  name: 'index',
  data() {
    return {
    }
  },
}
</script>

<style lamg="scss" scoped>
.container {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
  width: 100vh;
  width: 100vw;
  background-color: black;
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-weight: 300;
  font-size: 16px;
  color: #35495e;
}

.main_wrapper {
  position: absolute;
  top: 0;
  right: 0;
  left: 0;
  margin: auto;
  height: 50%;
  width: 100%;
}

.sub_wrapper {
  position: absolute;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
  width: calc(100vw - 4vh * 2);
  height: 38vh;
}

.aboutus {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  margin: auto;
  width: 200px;
  height: 100px;
  display: flex;
  align-items: center;
  color: white;
  font-size: 32px;
  font-weight: 900;
  z-index: 2;
}

.img_wrapper {
  position: absolute;
  right: 0;
  bottom: 0;
  width: 38vh;
  height: 38vh;
  z-index: 1;
  background-color: orangered;
}

.logo {
    position: absolute;
    top: 4vh;
    left: 4vh;
    margin: auto;
    width: calc(100vw - 4vh * 2 - 38vh);
    height: 3vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

.mikanLogo {
    height: calc(1.5vw + 1.5vh);
    margin: 0 4px 0 0;
}

.tunaLogo {
    height: calc(1.5vw + 1.5vh);
}


</style>
