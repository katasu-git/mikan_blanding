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
  height: 100%;
  width: 100%;
  padding: 8vmin;
}

@media screen and (min-height:320px) and (max-height:415px) and (max-width:737px){

/* iPhone5, iPhone6~8 & plus */

.main_wrapper {
  height: 100%;
  width: 100%;
  padding: 16vmin;
  overflow: scroll;
}

.sub_wrapper {
    position: relative;
    height: 96vmin;
    margin-top: 16vmin;
}

.img_wrapper {
    position: absolute;
    top: 0;
    right: 0;
    width: 96vmin;
    height: 96vmin;
    z-index: 1;
    background-color: orangered;
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
    font-size: 16vmin;
    font-weight: 900;
    white-space: nowrap;
    z-index: 2;
}

.logo {
    width: calc(100vw - 16vmin * 2 - 96vmin);
    height: 32vmin;
    display: flex;
    align-items: center;
    justify-content: center;
}

.mikanLogo {
    width: 37%;
    margin-right: 6%;
}

.tunaLogo {
    width: 57%;
}

}

@media screen and (min-height:320px) and (max-height:415px) and (min-width:811px) {

/* iPhoneX , XS Max */

.main_wrapper {
  height: 100%;
  width: 100%;
  padding: 16vmin;
  overflow: scroll;
}

.sub_wrapper {
    position: relative;
    height: 120vmin;
    margin-top: 16vmin;
}

.img_wrapper {
    position: absolute;
    top: 0;
    right: 0;
    width: 120vmin;
    height: 120vmin;
    z-index: 1;
    background-color: orangered;
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
    font-size: 16vmin;
    font-weight: 900;
    white-space: nowrap;
    z-index: 2;
}

.logo {
    width: calc(100vw - 16vmin * 2 - 120vmin);
    height: 32vmin;
    display: flex;
    align-items: center;
    justify-content: center;
}

.mikanLogo {
    width: 37%;
    margin-right: 6%;
}

.tunaLogo {
    width: 57%;
}

}

@media screen and (min-height:568px) {

  /* 縦画面 */

.sub_wrapper {
    position: relative;
    height: 64vmin;
    margin-top: 8vmin;
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
    font-size: 6vmin;
    font-weight: 900;
    white-space: nowrap;
    z-index: 2;
}

.img_wrapper {
    position: absolute;
    right: 0;
    width: 64vmin;
    height: 64vmin;
    z-index: 1;
    background-color: orangered;
}

.logo {
    width: calc(100vw - 8vmin * 2 - 64vmin);
    height: 16vmin;
    display: flex;
    align-items: center;
    justify-content: center;
}

.mikanLogo {
    width: 37%;
    margin-right: 6%;
}

.tunaLogo {
    width: 57%;
}

}


</style>
