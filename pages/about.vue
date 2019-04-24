<template>
  <div class="container">
      <div class="main_wrapper">
          <div class="logo">
              <img class="mikanLogo" src="../static/mikan_logo.png" />
              <img class="tunaLogo" src="../static/tuna_logo.png" />
          </div>
          <div class="contents_wrapper">
                <div class="grid_box">
                    <div class="about_box">ABOUT US</div>
                    <div class="img_box"></div>
                </div>
                <div class="grid_box"></div>
                <div class="grid_box"></div>
                <div class="grid_box"></div>
                <div class="grid_box"></div>
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
  bottom: 0;
  left: 0;
  margin: auto;
  height: 100%;
  width: 100%;
  padding: 24px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.logo {
    z-index: 2;
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

.contents_wrapper {
    width: 100%;
    max-width: 800px;
    height: 90%;
    margin: calc(2vh + 4vw) 0 0 0;
    padding: calc(1vh + 1vw);
    display: grid;
    /* minmax(最小,最大) */
    /* repeat(ボックスの数, ブロック幅) */
    /* grid-template-columns: 2fr 1fr → 2:1 で配置 */
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    grid-auto-rows: 320px;  /* 高さの最小 */
    grid-gap: calc(1vh + 1vw);
    overflow: auto;
}

.grid_box {
  min-height: 320px;
  position: relative;
}

.about_box {
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    margin: auto auto auto calc(-1vh - 1vw);
    width: 200px;
    height: 80px;
    display: flex;
    align-items: center;
    z-index: 2;
    color: white;
    font-size: 36px;
    font-weight: 900;
    white-space: nowrap;
}

.img_box {
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    margin: auto;
    height: calc(23vh + 23vw);
    width: calc(23vh + 23vw);
    max-width: 260px;
    max-height: 260px;
    background-color: chocolate;
}

</style>
