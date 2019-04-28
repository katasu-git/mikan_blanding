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
  width: 100vw;
  min-width: 320px;
  background-color: black;
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-weight: 300;
  font-size: 16px;
  overflow: auto; /*main_wrapperがはみ出したらスクロール*/
}

.main_wrapper {
  height: 100%;
  width: 100%;
  padding: 32px;
}

.logo {
  height: 40px;
  width: calc(100vw - 32px * 2 - 60vw);
  display: flex;
  align-items: center;
  justify-content: center;
}

.mikanLogo {
  width: 36%;
  margin-right: 8px;
}

.tunaLogo {
  width: 56%;
}

.sub_wrapper {
  position: relative;
  height: 60vw;
  width: calc(100vw - 32px * 2);
  margin: 32px 0;
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

.main_wrapper {
  padding: 64px;
}

.logo {
  height: 56px;
  width: calc(100vw - 64px * 2 - 60vw);
}

.sub_wrapper {
  width: calc(100vw - 64px * 2);
  margin: 64px 0;
}

}

@media screen and (min-width:768px) and (max-width:1024px) {

.main_wrapper {
  padding: 96px;
}

.logo {
  height: 72px;
  width: calc(100vw - 96px * 2 - 60vw);
}

.sub_wrapper {
  width: calc(100vw - 96px * 2);
  margin: 96px 0;
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
  width: 200px;
  max-width: 220px;
}

.sub_wrapper {
  max-height: 620px;
  max-width: 820px;
  margin: 128px 0;
}

.aboutus {
  max-width: 620px;
  max-height: 200px;
  font-size: 80px;
}

.img_wrapper {
  max-height: 620px;
  max-width: 620px;
}

}
</style>
