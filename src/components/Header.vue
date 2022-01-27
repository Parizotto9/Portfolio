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
      </section>
    </div>
    <section class="gradient"></section>
  </div>
</template>

<script>
export default {
  methods: {
    clicar() {},
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.logo {
  max-width: 80px;
}
.gradient {
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
  margin-right: 40px;
  margin-left: -40px;
}
.buttons {
  display: flex;
  align-items: center;
}
span {
  cursor: pointer;
  font-weight: 600;
  font-size: 1.6rem;
  margin-right: 80px;
}
.header {
  padding: 20px 30px;
  height: 500px;
  background: linear-gradient(180deg, #a9cadc 10%, #daf0fc 100%);
}
</style>
