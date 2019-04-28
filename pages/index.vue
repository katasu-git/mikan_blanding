<template>
  <div class="container">
      <div class="main_wrapper">
          <div class="logo">
              <img class="mikanLogo" alt="みかんの絵" src="../static/mikan_logo.png" />
              <img class="tunaLogo" alt="マグロの絵" src="../static/tuna_logo.png" />
          </div>
          <div class="title_img">
              <img class="nameLogo"  alt="みかんの国から" src="../static/name_logo.png" />
          </div>
          <div class="link_left">WORKS</div>
          <div class="link_right"><nuxt-link to="/about">ABOUT US</nuxt-link></div>
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
  overflow: auto; /*main_wrapperがはみ出したらスクロール*/
}

.main_wrapper {
  height: 100vh;
  width: 100%;
  padding: 32px;
  position: relative;
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

.nameLogo {
  width: calc(22vw + 22vh);
}

.title_img {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100px;
  width: 100%;
}

.link_left {
  position: absolute;
  bottom: 0;
  left: 0;
  margin: 32px;
  color: white;
  font-weight: 900;
}

.link_right {
  position: absolute;
  bottom: 0;
  right: 0;
  margin: 32px;
  color: white;
  font-weight: 900;
}

@media screen and (min-width:480px) {

.main_wrapper {
  padding: 64px;
}

.logo {
  height: 56px;
  width: calc(100vw - 64px * 2 - 60vw);
}

.link_right , .link_left {
  margin: 64px;
}

}

@media screen and (min-width:768px) and (max-width:1024px) {

.main_wrapper {
  padding: 96px;
}

.logo {
  height: 56px;
  width: calc(100vw - 96px * 2 - 60vw);
}

.link_right , .link_left {
  margin: 96px;
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
  height: 56px;
  width: calc(100vw - 128px * 2 - 60vw);
  max-width: 154px;
}

.mikanLogo {
  max-width: 56px;
}

.tunaLogo {
  max-width: 72px;
}

.link_right , .link_left {
  margin: 128px;
}

}

</style>
