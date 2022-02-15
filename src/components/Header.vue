<template>
  <div class="header">
    <div class="btnsarea">
      <section>
        <img alt="Logo" src="./../assets/logo.png" class="logo" />
      </section>
      <section class="buttons">
        <span @click="clicar('/')">Home</span>
        <!-- <button type="button"><span>Home</span></button> -->
        <span @click="clicar('/about')">About</span>
        <span @click="clicar('/skills')">Skills</span>
        <span @click="clicar('/portfolio')">Portfolio</span>
        <div class="divider"></div>
        <span @click="clicar('/portfolio')">Contact Me</span>
        <div class="drawer" @click="openDrawer()">
          <i class="fa fa-solid fa-bars"></i>
        </div>
      </section>
    </div>
    <div
      :class="drawer ? 'animation1' : 'none'"
      class="bg1"
      @click="openDrawer()"
    ></div>
    <div :class="drawer ? 'animation2' : 'none'" class="bg2">
      <h2>Home</h2>
      <h2 @click="clicar('/about')">About</h2>
      <h2>Skills</h2>
      <h2>Portfolio</h2>
      <h2>Contact Me</h2>
    </div>
    <section class="gradient"></section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      sizeScreen: null,
    };
  },
  computed: {
    innerWidth() {
      return window.innerWidth;
    },
  },
  methods: {
    clicar() {
      console.log(this.innerWidth, "alo");
    },
    openDrawer() {
      this.drawer = !this.drawer;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@media (max-width: 700px) {
  .bg1 {
    position: fixed;
    top: 0;
    width: 120vw;
    height: 100vh;
    z-index: 20;
    background-color: rgb(21, 40, 55, 0.5);
    transform: translateX(100vw);
    transition: 1.5s;
  }
  h2 {
    margin-top: 30px;
    font-size: 1.8rem;
    color: #04d7a2;
  }
  .bg2 {
    position: fixed;
    top: 0;
    display: flex;
    flex-direction: column;
    text-align: center;
    padding-top: 30px;
    align-content: center;
    right: 0;
    width: 65vw;
    height: 100vh;
    z-index: 21;
    background-color: #152837;
    transform: translateX(66vw);
    transition: 1.2s;
  }
  .animation1 {
    transform: translateX(-10vw);
  }
  .animation2 {
    transform: translateX(0vw);
  }
  span,
  .divider {
    display: none;
  }
  .logo {
    max-width: 60px;
    margin-left: 15%;
    margin-top: 2px;
  }
  .drawer {
    font-size: 2.4rem;
    color: #04d7a2;
    margin-right: 20px;
  }
  .header {
    padding: 15px 15px;
  }
}
@media (max-width: 850px) and (min-width: 700px) {
  .bg1,
  .bg2,
  .drawer {
    display: none;
  }
  span {
    font-size: 1.3rem;
    margin-right: 20px;
  }
  .divider {
    margin-right: 10px;
    margin-left: -10px;
  }
  .logo {
    max-width: 50px;
    margin-left: 15%;
    margin-top: 2px;
  }
  .header {
    padding: 15px 15px;
  }
}
@media (max-width: 1280px) and (min-width: 850px) {
  .bg1,
  .bg2,
  .drawer {
    display: none;
  }
  span {
    font-size: 1.4rem;
    margin-right: 40px;
  }
  .divider {
    margin-right: 20px;
    margin-left: -20px;
  }
  .logo {
    max-width: 70px;
    margin-left: 15%;
  }
  .header {
    padding: 15px 15px;
  }
}
@media (min-width: 1280px) {
  .bg1,
  .bg2,
  .drawer {
    display: none;
  }
  span {
    font-size: 1.6rem;
    margin-right: 60px;
  }
  .divider {
    margin-right: 30px;
    margin-left: -30px;
  }
  .logo {
    max-width: 80px;
    margin-left: 15%;
  }
  .header {
    padding: 20px 30px;
  }
}
.btnsarea {
  z-index: 10;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.divider {
  height: 50px;
  border-right: solid 2px #04d7a2;
}
.buttons {
  display: flex;
  align-items: center;
}
span {
  cursor: pointer;
  font-weight: 600;
}
.header {
  height: 500px;
  background: linear-gradient(180deg, #a9cadc 10%, #daf0fc 100%);
}
</style>
