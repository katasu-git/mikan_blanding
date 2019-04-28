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

html , body {
}

.container {
  height: 100vh;
  width: 100vw;
  min-width: 320px;
  background-color: black;
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-weight: 300;
  font-size: 16px;
}

.main_wrapper {
  height: 100%;
  width: 100%;
  padding: 32px;
}

.logo {
  position: absolute;
  height: 40px;
  display: flex;
}

.mikanLogo {
  height: 40px;
  margin-right: 8px;
}

.tunaLogo {
  height: 40px;
}

.sub_wrapper {
  position: relative;
  height: 60vw;
  width: 100%;
  margin-top: calc(40px + 32px);
}

.aboutus {
  position: absolute;
  top: 0;
  bottom: 0;
  margin: auto;
  height: 10vw;
  width: 60vw;
  display: flex;
  align-items: center;
  color: white;
  font-size: 8vw;
  font-weight: 900;
  z-index: 2;
}

.img_wrapper {
  position: absolute;
  top: 0;
  right: 0;
  height: 60vw;
  width: 60vw;
  z-index: 1;
  background-color: brown;
}

@media screen and (min-width:480px) {

.container {
  height: 250vh;
}

.main_wrapper {
  padding: 64px;
}

.logo {
  height: 56px;
}

.mikanLogo {
  height: 56px;
  margin-right: 8px;
}

.tunaLogo {
  height: 56px;
}

.sub_wrapper {
  height: 60vw;
  margin-top: calc(56px + 64px);
}

}

@media screen and (min-width:768px) and (max-width:1024px) {

.main_wrapper {
  padding: 96px;
}

.logo {
  height: 72px;
}

.mikanLogo {
  height: 72px;
  margin-right: 8px;
}

.tunaLogo {
  height: 72px;
}

.sub_wrapper {
  height: 60vw;
  margin-top: calc(72px + 96px);
}

}

@media screen and (min-width:1024px) {

.container {
  display: flex;
  align-items: center;
  justify-content: center;
}

.main_wrapper {
  padding: 128px;
  max-width: 1024px;
}

.logo {
  height: 72px;
}

.mikanLogo {
  height: 72px;
  margin-right: 8px;
}

.tunaLogo {
  height: 72px;
}

.sub_wrapper {
  max-height: 640px;
}

.aboutus {
  max-width: 640px;
  max-height: 200px;
  font-size: 80px;
}

.img_wrapper {
  max-height: 640px;
  max-width: 640px;
}

}
</style>
