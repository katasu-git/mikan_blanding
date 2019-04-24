<template>
  <div class="container">
      <div class="logo">
          <img class="mikanLogo" alt="みかんの絵" src="../static/mikan_logo.png" />
          <img class="tunaLogo" alt="マグロの絵" src="../static/tuna_logo.png" />
      </div>
      <div class="main_wrapper">
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
  letter-spacing: 1px;
}

.main_wrapper {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
  height: calc(100% - 80px);
  width: calc(100vw - 80px);
}

.logo {
  position: absolute;
  top: 24px;
  left: 24px;
  margin: auto;
  display: flex;
  align-items: center;
}

.mikanLogo {
  height: calc(3vw + 3vh);
  margin: 0 12px 0 0;
}

.tunaLogo {
  height: calc(3vw + 3vh);
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
  margin: auto;
  color: white;
  font-weight: 900;
}

.link_right {
  position: absolute;
  bottom: 0;
  right: 0;
  margin: auto;
  color: white;
  font-weight: 900;
}
</style>
